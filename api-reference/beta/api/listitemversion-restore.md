---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Восстановление предыдущей версии элемента списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b7c81022ebcb4f7afe02520c48f7cfbf103b2943
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983004"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="846cd-102">Восстановление предыдущей версии ресурса ListItem</span><span class="sxs-lookup"><span data-stu-id="846cd-102">Restore a previous version of a ListItem</span></span>

> <span data-ttu-id="846cd-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="846cd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="846cd-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="846cd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="846cd-105">Восстановление предыдущей версии ресурса ListItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="846cd-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="846cd-106">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.</span><span class="sxs-lookup"><span data-stu-id="846cd-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="846cd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="846cd-107">Permissions</span></span>

<span data-ttu-id="846cd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="846cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="846cd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="846cd-110">Permission type</span></span>             |         <span data-ttu-id="846cd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="846cd-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="846cd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="846cd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="846cd-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="846cd-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="846cd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="846cd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="846cd-115">Н/д</span><span class="sxs-lookup"><span data-stu-id="846cd-115">n/a</span></span>                                                          |
| <span data-ttu-id="846cd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="846cd-116">Application</span></span>                            | <span data-ttu-id="846cd-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="846cd-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="846cd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="846cd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="846cd-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="846cd-119">Request body</span></span>

<span data-ttu-id="846cd-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="846cd-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="846cd-121">Пример</span><span class="sxs-lookup"><span data-stu-id="846cd-121">Example</span></span>

<span data-ttu-id="846cd-122">В этом примере восстанавливается версия ресурса listItem, указанная пр `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="846cd-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="846cd-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="846cd-123">Response</span></span>

<span data-ttu-id="846cd-124">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="846cd-124">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
