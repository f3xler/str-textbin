# Vercel Environment Variables

This document describes the environment variables needed for the str-textbin project.

## Required Environment Variables

None! The textbin service uses the backend API at `https://str.pics` which doesn't require any API keys.

## Optional Environment Variables

### `API_BASE_URL` (Optional)
- **Default**: `https://str.pics`
- **Description**: The base URL for the backend API
- **Example**: `https://str.pics`

## How to Set Environment Variables in Vercel

1. Go to your Vercel project dashboard
2. Navigate to **Settings** → **Environment Variables**
3. Add the following variable (if you want to use a different API URL):
   - **Name**: `API_BASE_URL`
   - **Value**: `https://str.pics` (or your custom backend URL)
   - **Environment**: Production, Preview, Development (select all)
4. Redeploy your application for changes to take effect

## Note

The frontend uses `https://str.pics` as the default API base URL. If you need to change this, you can either:
- Set the `API_BASE_URL` environment variable and update the frontend code to use it
- Or directly modify the `API_BASE` constant in `index.html`

