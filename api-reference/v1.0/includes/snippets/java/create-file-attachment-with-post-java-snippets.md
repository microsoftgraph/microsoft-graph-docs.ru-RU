---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 020048fe477eadc08d15b09615341774e0eb5ea3f950fad77f804170e02eae48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57306570"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "Which quarter does that file cover? See my attachment.";
post.body = body;
LinkedList<Attachment> attachmentsList = new LinkedList<Attachment>();
FileAttachment attachments = new FileAttachment();
attachments.name = "Another file as attachment";
attachments.contentBytes = Base64.getDecoder().decode("VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu");
attachmentsList.add(attachments);
AttachmentCollectionResponse attachmentCollectionResponse = new AttachmentCollectionResponse();
attachmentCollectionResponse.value = attachmentsList;
AttachmentCollectionPage attachmentCollectionPage = new AttachmentCollectionPage(attachmentCollectionResponse, null);
post.attachments = attachmentCollectionPage;

graphClient.groups("1848753d-185d-4c08-a4e4-6ee40521d115").threads("AAQkADJUdfolA==")
    .reply(ConversationThreadReplyParameterSet
        .newBuilder()
        .withPost(post)
        .build())
    .buildRequest()
    .post();

```