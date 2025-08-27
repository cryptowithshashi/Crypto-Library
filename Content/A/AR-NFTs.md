# AR NFTs

## Overview
This guide covers augmented reality NFTs - digital assets that combine blockchain provenance with 3D/AR experiences. Essential for developers building immersive galleries, AR marketplaces, or spatial web applications that bridge physical and digital ownership.

## Why it matters
- Interoperability: Standardized 3D metadata enables cross-platform AR experiences across different galleries and viewers
- Discoverability: Proper metadata structure helps marketplaces surface AR-capable NFTs with rich preview functionality
- New experiences: Location-based and spatial anchoring creates novel interaction patterns beyond traditional 2D art viewing
- Monetization: AR galleries and immersive exhibitions open new revenue streams for artists and platform operators
- Future-proofing: Early adoption of spatial web standards positions projects for metaverse integration and WebXR growth

## Core concepts
Key technical concepts that enable AR NFT functionality and cross-platform compatibility.

- ERC-721/1155 metadata extensions for 3D - How to structure NFT metadata to reference 3D models and AR properties (Article)
- glTF/GLB format optimization - Industry standard for 3D web delivery with compression and streaming considerations (Doc)
- WebXR & WebAR implementation - Browser-native AR without app installs using device cameras and sensors (Doc)
- Spatial anchors & geo-location - Pinning digital content to real-world coordinates for location-based experiences (Paper)
- IPFS/Arweave hosting patterns - Decentralized storage strategies for large 3D assets with CDN fallbacks (Article)
- On-chain vs off-chain metadata - Gas optimization techniques and hybrid approaches for complex 3D asset references (Article)
- Mobile AR performance constraints - Polygon counts, texture sizes, and battery life considerations for mass adoption (Report)
- Cross-platform viewer compatibility - Ensuring GLB files work across iOS, Android, and web AR implementations (Doc)
- Provenance & authenticity verification - Cryptographic proofs for 3D model ownership and modification history (Paper)
- Privacy & geo-restrictions - Handling location data and content access in different jurisdictions (Report)

## Articles

* [Mozilla Hubs blog / guide](https://blog.mozilla.org/en/mozilla/mozilla-hubs-3d-vr-platform/) : Official blog explaining how to build galleries and use Spoke/Hubs.
* [Hubs client & tools (GitHub repo)](https://github.com/Hubs-Foundation/hubs) : The official GitHub repository for Hubs, useful for code and the Spoke editor.
* [WebXR fundamentals (Mozilla / MDN)](https://developer.mozilla.org/en-US/docs/Games/Techniques/3D_on_the_web/WebXR) : WebXR API reference and tutorials for building WebXR experiences.
* [OpenSea metadata & 3D support](https://docs.opensea.io/docs/metadata-standards) : Official documentation on metadata standards, including support for 3D models.
* [Google Scene Viewer guidance](https://developers.google.com/ar/develop/scene-viewer) : Google's guidance for preparing 3D models for AR delivery.
* [Practical glTF/GLB optimization overview](https://cloudinary.com/guides/image-formats/gltf-features-applications-and-5-essential-best-practices) : A platform-agnostic guide with tips for optimizing glTF/GLB files.
* [Pinata Docs - IPFS Pinning](https://docs.pinata.cloud/ipfs-101/what-is-ipfs-pinning) : An explanation of what IPFS pinning is and related best practices.
* [Pinata blog - Sharing 3D models with IPFS](https://medium.com/pinata/how-to-share-3d-models-with-ipfs-bb66df853962) : A tutorial on how to share 3D models using IPFS.
* [Niantic Lightship / SDK overview](https://www.nianticspatial.com/en/products/niantic-sdk) : An overview of the tools available for building location-based AR.
* [Lightship VPS docs](https://lightship.dev/docs/ardk/3.4/features/lightship_vps/) : Documentation for creating location-anchored AR experiences.
* [glTF 2.0 specification](https://registry.khronos.org/glTF/specs/2.0/glTF-2.0.html) : The authoritative technical specification for the glTF 2.0 format.
* [Khronos Asset Creation Guidelines](https://www.khronos.org/blog/introducing-asset-creation-guidelines-2.0-siggraph-2025) : Practical cross-platform best practices for creating glTF assets.
* [Ethereum gas docs](https://ethereum.org/en/developers/docs/gas/) : An explanation of how gas works and where costs come from on Ethereum.
* [Community discussion on gas optimisation](https://ethereum-magicians.org/t/help-with-optimising-gas-fees-for-on-chain-nfts/8671) : Practical tips and tradeoffs for optimizing on-chain NFT metadata.
* [Meta Horizon / MR design guidelines](https://developers.meta.com/horizon/design/mr-design-guideline/) : UX principles for designing immersive mixed reality experiences.
* [Meta / Reality Labs design principles](https://tech.facebook.com/reality-labs/) : Research posts and design principles from Meta's Reality Labs.



## Docs

* [glTF 2.0 Specification - Official spec (PDF)](https://registry.khronos.org/glTF/specs/2.0/glTF-2.0.pdf) : The authoritative spec for glTF 2.0.
* [WebXR Device API (spec)](https://www.w3.org/TR/webxr/) : The official browser AR/VR Device API specification.
* [ERC-721: Non-Fungible Token Standard (EIP-721)](https://eips.ethereum.org/EIPS/eip-721) : The official NFT metadata and contract API standard.
* [<model-viewer> Web Component (docs)](https://modelviewer.dev/) : An embeddable 3D + AR web component with documentation.
* [WebAR / WebXR Implementation Guide (MDN)](https://developer.mozilla.org/en-US/docs/Games/Techniques/3D_on_the_web/WebXR) : WebXR guidance and WebAR best practices on MDN.
* [IPFS HTTP Gateway API (reference)](https://docs.ipfs.tech/reference/http/gateway/) : The IPFS gateway and HTTP API reference.
* [Arweave - Developer Docs](https://docs.arweave.org/developers) : Permanent data storage and HTTP API docs for developers.
* [three.js - WebXR / WebXRManager docs](https://threejs.org/docs/api/en/renderers/webxr/WebXRManager.html) : WebXR integration and API reference for three.js.
* [WebXR AR Module (AR-specific spec)](https://www.w3.org/TR/webxr-ar-module-1/) : WebXR AR Module Level 1, useful for AR-only features.

## Research Papers
* [Immersive Web (WebXR) developer site](https://immersiveweb.dev/) : The closest official hub for WebXR samples, guides, and status updates.
* [XR Association - State of the Industry Report 2024](https://xra.org/xr-association-releases-state-of-the-industry-report-with-highlights-from-2024-and-a-look-ahead-to-2025/) : A broader industry report covering XR metrics for 2024.
* [Stanford news / VHI lab summary of spatial/mixed-reality research](https://news.stanford.edu/stories/2024/02/researchers-take-new-mixed-reality-headsets-spin) : Stanford's coverage on spatial and mixed-reality research.
* [CS 12SI Spatial Computing Workshop](https://explorecourses.stanford.edu/search?academicYear=20242025&filter-coursestatus-Active=on&q=CS+12SI%3A+Spatial+Computing+Workshop&view=catalog) : Stanford course pages that cover spatial computing and HCI.
* [arXiv review - “Spatial Computing: Concept, Applications, Challenges and Future …”](https://arxiv.org/abs/2402.07912) : A broad academic review on spatial computing that covers UX patterns and digital collectibles.
* [Unity Performance Testing package docs](https://docs.unity3d.com/Packages/com.unity.test-framework.performance%403.1/manual/index.html) : Unity's official resources for benchmarking and performance testing.
* [Unity guidance on performance benchmarks](https://unity.com/blog/engine-platform/performance-benchmarking-in-unity-how-to-get-started) : Best practices for setting up performance benchmarks in Unity.
* [Unity Gaming Report / Industry resources](https://unity.com/resources/gaming-report-2024) : Unity's industry reports that include performance and optimization findings.
* [MIT Media Lab research landing](https://www.media.mit.edu/research/?filter=everything&tag=blockchain) : A hub for MIT Media Lab research, filterable by "blockchain" and spatial research.
* [MIT Media Lab general research portal](https://www.media.mit.edu/) : Useful for finding related projects and papers.
* [DappRadar industry & NFT reports landing page](https://dappradar.com/reports) : The official landing page for DappRadar's reports.
* [DappRadar blog / industry-overview posts](https://dappradar.com/blog/dapp-industry-report-2024-overview) : 2024 industry highlights and market stats.
* [Protocol Labs Research hub](https://research.protocol.ai/) : The official research and IPFS/Filecoin work from Protocol Labs.
* [Protocol Labs / IPFS docs & blog](https://docs.ipfs.tech/) : Practical background on IPFS/File distribution.
* [Magic Leap product/dev pages](https://www.magicleap.com/magic-leap-2) : Official pages describing device features and cross-platform development.
* [Unity / AR Foundation sessions & resources](https://www.youtube.com/watch?v=1dOMZNYKG_I) : Useful for compatibility strategy across devices.
* [PrivStats: Privacy and Accountability for Location-based Aggregate Statistics](https://people.eecs.berkeley.edu/~raluca/PrivStats.pdf) : Berkeley research on privacy for location data and privacy-preserving aggregates.

## Github Repositories

| Requested Repo | Status & Alternatives | Notes |
| :--- | :--- | :--- |
| `ethereum/ar-nft-gallery` (⭐234) | No exact repo found. Closest alternative: [bkrem/react-nft-gallery](https://github.com/bkrem/react-nft-gallery). | Many NFT gallery projects exist under different owners — use the “nft-gallery” topic or search to find production-ready examples. |
| `KhronosGroup/glTF-Validator` (⭐1.2k) | [Found at github.com/KhronosGroup/glTF-Validator](https://github.com/KhronosGroup/glTF-Validator). | Official validator for glTF/GLB assets (live drag-and-drop site + CLI/NPM packages). |
| `mozilla/webxr-nft-viewer` (⭐89) | No exact repo found. Closest Mozilla repos: [mozilla-mobile/webxr-ios](https://github.com/mozilla-mobile/webxr-ios) and [mozilla/webxr-polyfill](https://github.com/mozilla/webxr-polyfill). | Mozilla’s WebXR examples & viewer code are split across repos (iOS viewer, polyfills, emulator, etc.). |
| `pinata-cloud/ipfs-3d-uploader` (⭐156) | No exact repo found. Relevant links: [PinataCloud Org](https://github.com/PinataCloud), [ipfs-gateway-tools](https://github.com/PinataCloud/ipfs-gateway-tools), and [CI→IPFS blog tutorial](https://pinata.cloud/blog/how-to-use-github-actions-with-ipfs/). | Pinata has SDKs, tools and tutorials rather than a repo with that exact name — check their org for upload/pinning helpers. |
| `openzeppelin/spatial-nft-contracts` (⭐67) | No exact repo found. Use the official contracts library: [OpenZeppelin/openzeppelin-contracts](https://github.com/OpenZeppelin/openzeppelin-contracts). | OpenZeppelin provides ERC-721/1155 templates; “spatial” NFT examples are usually community forks or application-specific. |
| `opensea/ar-metadata-tools` (⭐43) | No exact repo found. Relevant links: [OpenSea Org](https://github.com/projectopensea), community [metadata helper](https://github.com/seascapenetwork/opensea-metadata), and [metadata docs](https://docs.opensea.io/docs/metadata-standards). | OpenSea publishes docs and some tooling; many metadata utilities are community repos or in-house tools not published under that exact name. |
| `google/mobile-ar-optimizer` (⭐178) | No exact repo found. Relevant Google AR repos: [arcore-android-sdk](https://github.com/google-ar/arcore-android-sdk) and [google/filament](https://github.com/google/filament) (renderer/optimizations). | Google tends to publish AR SDKs (ARCore) and rendering tools (Filament) rather than a single “mobile-ar-optimizer” repo. |
| `niantic/location-ar-nfts` (⭐91) | No exact repo found. Relevant links: [Niantic Org](https://github.com/nianticlabs) and [ardk-samples](https://github.com/niantic-lightship/ardk-samples). | Niantic’s sample projects and Lightship SDK are the right starting point for GPS-anchored experiences; specific NFT demos are usually community-built on top of Lightship. |


## Galleries & marketplace integrations
Notable platforms supporting AR NFT viewing and exhibition experiences.

* [Cyber](https://cyber.co) : Browser-based AR gallery with social features.
* [Spatial](https://spatial.io) : Virtual worlds with NFT integration and mobile AR.
* [Oncyber](https://oncyber.io) : Web3 gallery builder with glTF support.
* [Museum of Other Realities](https://museumor.com) : VR/AR exhibition space for digital art.
* [SuperRare AR](https://superrare.com/ar) : Curated AR exhibitions with location anchoring.
* [Foundation Galleries](https://foundation.app/galleries) : 3D NFT display with WebXR viewer.
* [Async Art AR](https://async.art/ar) : Programmable AR art with blockchain interaction.
* [Voxels](https://voxels.com) : Metaverse platform with NFT gallery districts.


## Tools / Libraries / Viewers

- **model-viewer:** Google web component for embedding 3D/AR content with iOS Quick Look integration
- **three.js WebXR:** Low-level 3D library with full WebXR API access for custom AR experiences
- **Babylon.js WebXR:** Microsoft 3D engine with built-in AR scene management and physics
- **8th Wall WebAR:** Computer vision SDK for marker-based and SLAM tracking (paywalled)
- **A-Frame:** Mozilla declarative framework for WebXR with component architecture
- **glTF-Transform:** Node.js toolkit for programmatic glTF optimization and validation
- **Draco 3D compression:** Google mesh compression for reduced file sizes
- **Sketchfab Viewer API:** Embeddable 3D viewer with AR mode for existing model libraries



## Books recommended to read

* [The Spatial Web by Gabriel Rene](https://annas-archive.org/md5/576d638f9d14ee236f47732f91fcd15d) : Comprehensive overview of AR/VR infrastructure and economic models.
* [WebXR Programming by Rakesh Baruah](https://annas-archive.org/md5/8f4e62e3353ca76eb1868a46fecf803e) : Technical deep-dive into browser-based AR development.
* [Designing Reality by Brockwell & Hart](https://annas-archive.org/md5/20ed28c56a3969305d65b7551a711448) : UX principles for spatial computing and mixed reality interfaces.
* [The Metaverse Primer by Matthew Ball](https://annas-archive.org/md5/047591188726049b611616bb509c25b4) : Strategic analysis of virtual world economics and NFT integration.
* [3D Graphics for Web Developers by Tony Parisi](https://annas-archive.org/md5/c9e6443d1a5a57048ba5806663aa9d66) : Practical guide to WebGL, three.js, and 3D asset pipelines.

## Quick start - sample metadata & delivery


### Example NFT metadata with 3D asset

```bash
{
  "name": "Spatial Sculpture #001",
  "description": "Interactive 3D sculpture with AR capabilities",
  "image": "ipfs://QmThumbnail2D...",
  "animation_url": "ipfs://QmModel3D.glb",
  "properties": {
    "model": {
      "format": "glb",
      "size": "2.4MB",
      "vertices": 15420
    },
    "ar": {
      "auto_rotate": true,
      "scale": 1.0,
      "placement": "horizontal-plane"
    }
  }
}
```
### AR metadata extension (recommended practice)

```bash
{
  "ar_metadata": {
    "anchor_type": "plane_detection",
    "initial_scale": [1.0, 1.0, 1.0],
    "bounding_box": {
      "width": 2.5,
      "height": 3.0,
      "depth": 2.5
    },
    "interactions": ["tap_to_animate", "pinch_to_scale"],
    "requires_camera": true,
    "min_lighting": 100
  }
}
```

### IPFS upload with Pinata

```bash
curl -X POST "https://api.pinata.cloud/pinning/pinFileToIPFS" \
  -H "Authorization: Bearer YOUR_JWT_TOKEN" \
  -F 'file=@sculpture.glb' \
  -F 'pinataMetadata={"name":"Sculpture GLB"}'
  ```
> [!HOSTING NOTE]
> Use IPFS/Arweave for permanence with CDN caching (Cloudflare/Fastly) for performance. Most marketplaces read animation_url field to detect 3D content and automatically render AR preview buttons.


> [!NOTE]
> Please be advised that the direct download links for the books in the crypto library repository are associated with a third-party website. If this website is unavailable, it may be due to regulatory changes.
To ensure uninterrupted access to these resources, a public Google Drive folder containing all the books has been created. The access link can be found in the `Books.md` file within the repository. This shared drive is open to all users for educational and informational purposes.


## Disclaimer

This guide provides general information about API security practices and is intended for educational purposes only. It should not be considered as legal, compliance, or professional security advice. Organizations should consult with qualified security professionals and conduct thorough security assessments to address their specific requirements and regulatory obligations.

## License

This resource is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). Content is for educational and informational purposes only. Always consult qualified legal counsel for specific compliance requirements.

Regulatory requirements change frequently. Verify current requirements with appropriate authorities. Contributors are not responsible for the accuracy, completeness, or currency of external resources.

- Last Updated: August 27, 2025
- Maintainer: cryptowithshashisupport@gmail.com
- Contributors: 0

