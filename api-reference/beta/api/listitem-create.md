---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Создание записи в списке SharePoint
localization_priority: Normal
ms.openlocfilehash: 8268ec362a2ce60686f0ef2467243799cd650a9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822549"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="bfbe6-102">Создание элемента в списке</span><span class="sxs-lookup"><span data-stu-id="bfbe6-102">Create a new item in a list</span></span>

> <span data-ttu-id="bfbe6-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bfbe6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfbe6-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfbe6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfbe6-105">Создание элемента [listItem][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="bfbe6-105">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="bfbe6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfbe6-106">Permissions</span></span>

<span data-ttu-id="bfbe6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfbe6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfbe6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfbe6-109">Permission type</span></span>      | <span data-ttu-id="bfbe6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfbe6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfbe6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfbe6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bfbe6-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfbe6-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bfbe6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfbe6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfbe6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfbe6-114">Not supported.</span></span>    |
|<span data-ttu-id="bfbe6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfbe6-115">Application</span></span> | <span data-ttu-id="bfbe6-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfbe6-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfbe6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfbe6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="bfbe6-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bfbe6-118">Request body</span></span>

<span data-ttu-id="bfbe6-119">В теле запроса укажите представление ресурса [listItem][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfbe6-119">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="bfbe6-120">Пример</span><span class="sxs-lookup"><span data-stu-id="bfbe6-120">Example</span></span>

<span data-ttu-id="bfbe6-121">В примере ниже показано, как создать элемент списка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="bfbe6-121">Here is an example of how to create a new generic list item.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="bfbe6-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="bfbe6-122">Response</span></span>

<span data-ttu-id="bfbe6-123">При успешном выполнении этот метод возвращает объект [listItem][] для созданного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bfbe6-123">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

<span data-ttu-id="bfbe6-124">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="bfbe6-124">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="bfbe6-125">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bfbe6-125">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create"
} -->
