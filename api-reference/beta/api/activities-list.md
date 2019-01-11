---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: Файл действий
localization_priority: Normal
ms.openlocfilehash: 55719340eb8baa565c79802403909b66ee5a4e49
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833770"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="dc045-102">Перечисление действий (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="dc045-102">Enumerate activities (preview)</span></span>

> <span data-ttu-id="dc045-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc045-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc045-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc045-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc045-105">В этой статье рассказывается, как создать список последних [действий][], выполненных над элементом или в иерархии.</span><span class="sxs-lookup"><span data-stu-id="dc045-105">List the recent [activities][] that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="dc045-106">**Примечание.** Ресурс activities представлен в предварительной версии и пока не доступен всем клиентам.</span><span class="sxs-lookup"><span data-stu-id="dc045-106">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="dc045-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc045-108">Permissions</span></span>

<span data-ttu-id="dc045-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc045-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc045-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc045-111">Permission type</span></span>                        | <span data-ttu-id="dc045-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc045-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="dc045-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc045-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc045-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc045-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="dc045-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc045-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc045-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc045-116">Not supported.</span></span>
|<span data-ttu-id="dc045-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc045-117">Application</span></span>                            | <span data-ttu-id="dc045-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc045-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="dc045-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc045-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="dc045-120">Пример</span><span class="sxs-lookup"><span data-stu-id="dc045-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dc045-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc045-121">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="dc045-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc045-122">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites"
} -->
