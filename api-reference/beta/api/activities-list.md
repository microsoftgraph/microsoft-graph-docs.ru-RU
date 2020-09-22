---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: Действия с файлами
description: В этой статье рассказывается, как создать список последних действий, выполненных над элементом или в иерархии.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: e75043fe3d91754902b078d6bd88b1227295587a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983440"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="a4e5a-103">Перечисление действий (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="a4e5a-103">Enumerate activities (preview)</span></span>

<span data-ttu-id="a4e5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4e5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4e5a-105">В этой статье рассказывается, как создать список последних [действий](../resources/itemactivity.md), выполненных над элементом или в иерархии.</span><span class="sxs-lookup"><span data-stu-id="a4e5a-105">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="a4e5a-106">**Примечание.** Ресурс activities представлен в предварительной версии и пока не доступен всем клиентам.</span><span class="sxs-lookup"><span data-stu-id="a4e5a-106">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="a4e5a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4e5a-107">Permissions</span></span>

<span data-ttu-id="a4e5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4e5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4e5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4e5a-110">Permission type</span></span>                        | <span data-ttu-id="a4e5a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4e5a-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="a4e5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4e5a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4e5a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e5a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="a4e5a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4e5a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4e5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4e5a-115">Not supported.</span></span>
|<span data-ttu-id="a4e5a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4e5a-116">Application</span></span>                            | <span data-ttu-id="a4e5a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e5a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a4e5a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4e5a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="a4e5a-119">Пример</span><span class="sxs-lookup"><span data-stu-id="a4e5a-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a4e5a-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4e5a-120">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a4e5a-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4e5a-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-activities" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/activities
```
# <a name="c"></a>[<span data-ttu-id="a4e5a-122">C#</span><span class="sxs-lookup"><span data-stu-id="a4e5a-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-activities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4e5a-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4e5a-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-activities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4e5a-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4e5a-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-activities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4e5a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4e5a-125">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivity)", "truncated": true } -->

```json
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


