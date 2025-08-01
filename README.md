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

type AvatarSource = {
  media?: string;
  type?: "apng" | "avif" | "gif" | "jpeg" | "png" | "svg+xml" | "webp";
} & (
  | {
      src: string;
      srcset?: string;
    }
  | {
      src?: string;
      srcset: string;
    }
);
```
