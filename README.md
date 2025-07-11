# friends

No new friends.

## TypeScript Definition

```typescript
interface Friend {
  avatar: Avatar;
  url: string;
  name: string;
  description?: string;
  lang: string;
  hrefLang: string;
}

type Avatar =
  | string
  | {
      src: string;
      srcset?: string;
      sources?: AvatarSource[];
    };

interface AvatarSource {
  media?: string;
  srcset: string;
  type?: "apng" | "avif" | "gif" | "jpeg" | "png" | "svg+xml" | "webp";
}
```
