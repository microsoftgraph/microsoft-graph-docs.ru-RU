---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Создание списка SharePoint
ms.openlocfilehash: a1e247722e9e8874a78a1951619e08bff9bd36e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082193"
---
# <a name="create-a-new-list"></a><span data-ttu-id="eab92-102">Создание списка</span><span class="sxs-lookup"><span data-stu-id="eab92-102">Create a new list</span></span>

> <span data-ttu-id="eab92-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eab92-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eab92-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eab92-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eab92-105">Создание [списка][] на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="eab92-105">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="eab92-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eab92-106">Permissions</span></span>

<span data-ttu-id="eab92-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eab92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="eab92-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eab92-109">Permission type</span></span>             | <span data-ttu-id="eab92-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eab92-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="eab92-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eab92-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eab92-112">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="eab92-112">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="eab92-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eab92-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eab92-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eab92-114">Not supported.</span></span>                              |
| <span data-ttu-id="eab92-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eab92-115">Application</span></span>                            | <span data-ttu-id="eab92-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eab92-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="eab92-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eab92-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="eab92-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eab92-118">Request body</span></span>

<span data-ttu-id="eab92-119">В теле запроса укажите представление ресурса [списка][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eab92-119">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="eab92-120">Пример</span><span class="sxs-lookup"><span data-stu-id="eab92-120">Example</span></span>

<span data-ttu-id="eab92-121">В примере ниже показано, как создать список общего назначения.</span><span class="sxs-lookup"><span data-stu-id="eab92-121">Here is an example of how to create a new generic list.</span></span>

<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "name": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```

<span data-ttu-id="eab92-122">**Примечание.** Настраиваемые столбцы являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="eab92-122">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="eab92-123">Помимо столбцов, указанных здесь, в создаваемых списках используются столбцы, заданные в соответствующем **шаблоне**.</span><span class="sxs-lookup"><span data-stu-id="eab92-123">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="eab92-124">Если аспект или **шаблон** **списка** не указаны, то по умолчанию для списка используется шаблон `genericList`, включающий столбец _Title_ (Название).</span><span class="sxs-lookup"><span data-stu-id="eab92-124">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="eab92-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="eab92-125">Response</span></span>

<span data-ttu-id="eab92-126">При успешном выполнении этот метод возвращает объект [списка][] для вновь созданного списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="eab92-126">If successful, this method returns a [list][] in the response body for the created list.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
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

<span data-ttu-id="eab92-127">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="eab92-127">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="eab92-128">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="eab92-128">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
