---
author: daspek
ms.date: 09/10/2017
title: Действия файлов
description: В этой статье рассказывается, как создать список последних действий, выполненных над элементом или в иерархии.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: f345551f4685023581eea58fa2615e9c723303f5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472260"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="25c81-103">Перечисление действий (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="25c81-103">Enumerate activities (preview)</span></span>

<span data-ttu-id="25c81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25c81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25c81-105">В этой статье рассказывается, как создать список последних [действий](../resources/itemactivity.md), выполненных над элементом или в иерархии.</span><span class="sxs-lookup"><span data-stu-id="25c81-105">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="25c81-106">**Примечание.** Ресурс activities представлен в предварительной версии и пока не доступен всем клиентам.</span><span class="sxs-lookup"><span data-stu-id="25c81-106">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="25c81-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25c81-107">Permissions</span></span>

<span data-ttu-id="25c81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25c81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25c81-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25c81-110">Permission type</span></span>                        | <span data-ttu-id="25c81-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25c81-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="25c81-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25c81-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="25c81-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c81-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="25c81-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25c81-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25c81-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25c81-115">Not supported.</span></span>
|<span data-ttu-id="25c81-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25c81-116">Application</span></span>                            | <span data-ttu-id="25c81-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c81-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="25c81-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25c81-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="25c81-119">Пример</span><span class="sxs-lookup"><span data-stu-id="25c81-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="25c81-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="25c81-120">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="25c81-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="25c81-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-activities" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/activities
```
# <a name="c"></a>[<span data-ttu-id="25c81-122">C#</span><span class="sxs-lookup"><span data-stu-id="25c81-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-activities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25c81-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25c81-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-activities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25c81-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25c81-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-activities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25c81-125">Java</span><span class="sxs-lookup"><span data-stu-id="25c81-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-activities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="25c81-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="25c81-126">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivity)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "action": {
                "comment": {}
            },
            "actor": {
                "user": {
                    "displayName": "Xavier Wilke"
                }
            },
            "id": "EJalEvjV1EgIYFQAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-29T18:34:40Z"
            }
        },
        {
            "action": {
                "edit": {},
                "version": {
                    "newVersion": "2.0"
                }
            },
            "actor": {
                "user": {
                    "displayName": "Judith Clemons"
                }
            },
            "id": "cInT6/fV1EgFYFQAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-29T16:23:35Z"
            }
        },
        {
            "action": {
                "mention": {
                    "mentionees": [
                        {
                            "user": {
                                "displayName": "Judith Clemons"
                            }
                        }
                    ]
                }
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "EBJa0vPV1EjFX1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:14:14Z"
            }
        },
        {
            "action": {
                "rename": {
                    "oldName": "Document2.docx"
                }
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "QFJFlfPV1Ei/X1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:12:32Z"
            }
        },
        {
            "action": {
                "create": {}
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "IJydkPPV1Ei9X1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:02:24Z"
            }
        }
    ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
  ]
}
-->


