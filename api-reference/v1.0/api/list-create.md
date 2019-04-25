---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7faabe9bddc806d4c416ebed439592ec8630e8af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568098"
---
# <a name="create-a-new-list"></a><span data-ttu-id="77056-102">Создание списка</span><span class="sxs-lookup"><span data-stu-id="77056-102">Create a new list</span></span>

<span data-ttu-id="77056-103">Создание [списка][] на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="77056-103">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="77056-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77056-104">Permissions</span></span>

<span data-ttu-id="77056-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77056-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="77056-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77056-107">Permission type</span></span>             | <span data-ttu-id="77056-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77056-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="77056-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77056-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="77056-110">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="77056-110">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="77056-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77056-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77056-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77056-112">Not supported.</span></span>                              |
| <span data-ttu-id="77056-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77056-113">Application</span></span>                            | <span data-ttu-id="77056-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77056-114">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="77056-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77056-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="77056-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77056-116">Request body</span></span>

<span data-ttu-id="77056-117">В теле запроса укажите представление ресурса [списка][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77056-117">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="77056-118">Пример</span><span class="sxs-lookup"><span data-stu-id="77056-118">Example</span></span>

<span data-ttu-id="77056-119">В примере ниже показано, как создать список общего назначения.</span><span class="sxs-lookup"><span data-stu-id="77056-119">Here is an example of how to create a new generic list.</span></span>

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

<span data-ttu-id="77056-120">**Примечание.** Настраиваемые столбцы являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="77056-120">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="77056-121">Помимо столбцов, указанных здесь, в создаваемых списках используются столбцы, заданные в соответствующем **шаблоне**.</span><span class="sxs-lookup"><span data-stu-id="77056-121">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="77056-122">Если аспект или **шаблон** **списка** не указаны, то по умолчанию для списка используется шаблон `genericList`, включающий столбец _Title_ (Название).</span><span class="sxs-lookup"><span data-stu-id="77056-122">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="77056-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="77056-123">Response</span></span>

<span data-ttu-id="77056-124">При успешном выполнении этот метод возвращает объект [списка][] для вновь созданного списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="77056-124">If successful, this method returns a [list][] in the response body for the created list.</span></span>

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

<span data-ttu-id="77056-125">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="77056-125">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="77056-126">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="77056-126">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
