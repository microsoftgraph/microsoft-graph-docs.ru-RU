---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: Действия с файлами
description: В этой статье рассказывается, как создать список последних действий, выполненных над элементом или в иерархии.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 075f4f3df4e16e23fa3f90cb7de70a502b1d0aae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945937"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="11968-103">Перечисление действий (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="11968-103">Enumerate activities (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11968-104">В этой статье рассказывается, как создать список последних [действий](../resources/itemactivity.md), выполненных над элементом или в иерархии.</span><span class="sxs-lookup"><span data-stu-id="11968-104">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="11968-105">**Примечание.** Ресурс activities представлен в предварительной версии и пока не доступен всем клиентам.</span><span class="sxs-lookup"><span data-stu-id="11968-105">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="11968-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11968-106">Permissions</span></span>

<span data-ttu-id="11968-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11968-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11968-109">Permission type</span></span>                        | <span data-ttu-id="11968-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11968-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="11968-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11968-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11968-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11968-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="11968-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11968-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11968-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11968-114">Not supported.</span></span>
|<span data-ttu-id="11968-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11968-115">Application</span></span>                            | <span data-ttu-id="11968-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11968-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="11968-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11968-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="11968-118">Пример</span><span class="sxs-lookup"><span data-stu-id="11968-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="11968-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="11968-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="11968-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="11968-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="11968-121">C#</span><span class="sxs-lookup"><span data-stu-id="11968-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-activities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11968-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="11968-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-activities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="11968-123">Цель — C</span><span class="sxs-lookup"><span data-stu-id="11968-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-activities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="11968-124">Java</span><span class="sxs-lookup"><span data-stu-id="11968-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-activities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="11968-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="11968-125">Response</span></span>

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
