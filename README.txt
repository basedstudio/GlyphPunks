Based Glyphs Punks — Final deploy package
============================================

Files:
- index.html              (mint page + social links)
- public/assets/*         (placeholder logo & icons)
- .well-known/farcaster.json  (domain manifest placeholder)

INSTRUCTIONS:
1. Edit '.well-known/farcaster.json':
   - Replace "owner_fid" with your Farcaster FID (get from Warpcast profile)
   - Replace "signature" with the real signed manifest if you generate it via Farcaster tool (recommended).
   - Optionally change "domain" to your deployed vercel domain if different.

2. (Optional) Replace images in public/assets/ with real logo/icons.

3. Deploy to Vercel:
   - Go to https://vercel.com/new
   - Drag & drop this folder (based-glyphs-punks-final)
   - Deploy

4. Verify manifest on Farcaster:
   - Visit the Domain Manifest tool in Farcaster (Warpcast dev settings)
   - Enter your domain (e.g. based-glyphs-punks.vercel.app)
   - Use 'Check domain status' to verify
   - If you used Farcaster's tool to generate signed manifest, paste the manifest JSON into their Verify tool or upload the file and check status.

Notes:
- Do NOT publish private keys into repository or manifest. The signature must be created by signing the manifest payload with your Farcaster custody key using Farcaster tooling.
- If you want, I can also generate the signed manifest instructions or a Node script to create the signature locally (you keep the private key secret).
