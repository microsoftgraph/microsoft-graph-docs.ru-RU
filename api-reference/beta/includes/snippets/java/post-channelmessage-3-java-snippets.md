---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b20106bfa927a2e7cdb0e25bd76895eb3c72d2e57206c26a3348dc42ee950c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57257869"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
chatMessage.createdDateTime = OffsetDateTimeSerializer.deserialize("2019-02-04T19:58:15.511Z");
ChatMessageFromIdentitySet from = new ChatMessageFromIdentitySet();
Identity user = new Identity();
user.id = "id-value";
user.displayName = "John Doe";
user.userIdentityType = TeamworkUserIdentityType.AAD_USER;
from.user = user;
chatMessage.from = from;
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "<div><div>\n<div><span><img height=\"250\" src=\"../hostedContents/1/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>";
chatMessage.body = body;
LinkedList<ChatMessageHostedContent> hostedContentsList = new LinkedList<ChatMessageHostedContent>();
ChatMessageHostedContent hostedContents = new ChatMessageHostedContent();
hostedContents.additionalDataManager().put("@microsoft.graph.temporaryId", new JsonPrimitive("1"));
hostedContents.contentBytes = Base64.getDecoder().decode("iVBORw0KGgoAAAANSUhEUgAAANcAAAExCAYAAADvFzeeAAAXjklEQVR4Ae2d/XNU1RnH+9e0FFrA0RCIyaS8hRA0HV5KbS1gHRgVpjMClY4GHJ3yYm1HCmXaWttaaZUZtIIFKYi8lFAkvOQ9u5vN225IARVBbX9/Os9NbrLZbMjmhCfJPX5+2Lmb3T25y3O+n/M599x7w9f+++UXwoMakIF7n4GvUdR7X1RqSk01A8CFuZm5GGUAuIwKi72wF3ABF+YyygBwGRUWc2Eu4AIuzGWUAeAyKizmwlzABVyYyygDwGVUWMyFuYALuDCXUQaAy6iwmAtzARdwfWXMdeuzT+TGxz3Sfb1LunrapL07IW3pePDQ5/qavqef0c+OdYAELuAac4jGGkLL9rdvfyo9N9ODQAqBGmmrwGlb/R0u3xG4gMspOC5hG882CoRaaCSA8n1ff9doIQMu4PIOrus3u+8ZVNnw6e/Od5AALuDKOyz5hmqiPnfnzi1J9bSbgRWCpvvQfY307wQu4BoxJCOFaDK8rwsQmQsUIQhWW93XSIsewAVckYdLQ24F0Ui/926AARdwRRounZ6Np7GyYdN9DzdFBC7gijRc43GMlQ1U9s/6HXJNjYELuHI<<-----Removed----->>>>");
hostedContents.contentType = "image/png";
hostedContentsList.add(hostedContents);
ChatMessageHostedContentCollectionResponse chatMessageHostedContentCollectionResponse = new ChatMessageHostedContentCollectionResponse();
chatMessageHostedContentCollectionResponse.value = hostedContentsList;
ChatMessageHostedContentCollectionPage chatMessageHostedContentCollectionPage = new ChatMessageHostedContentCollectionPage(chatMessageHostedContentCollectionResponse, null);
chatMessage.hostedContents = chatMessageHostedContentCollectionPage;

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5").channels("19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2").messages()
    .buildRequest()
    .post(chatMessage);

```