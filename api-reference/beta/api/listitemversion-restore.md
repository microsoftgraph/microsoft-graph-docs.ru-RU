---
author: JeremyKelley
description: Восстановление предыдущей версии ресурса ListItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.
ms.date: 09/10/2017
title: Восстановление предыдущей версии элемента списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f70ae287b787a30e835c9fb8403b32b4f808c1ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971954"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="0ad70-104">Восстановление предыдущей версии ресурса ListItem</span><span class="sxs-lookup"><span data-stu-id="0ad70-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="0ad70-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ad70-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ad70-106">Восстановление предыдущей версии ресурса ListItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="0ad70-106">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="0ad70-107">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.</span><span class="sxs-lookup"><span data-stu-id="0ad70-107">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ad70-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ad70-108">Permissions</span></span>

<span data-ttu-id="0ad70-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ad70-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="0ad70-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ad70-111">Permission type</span></span>             |         <span data-ttu-id="0ad70-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ad70-112">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="0ad70-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ad70-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ad70-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0ad70-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="0ad70-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ad70-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ad70-116">Н/д</span><span class="sxs-lookup"><span data-stu-id="0ad70-116">n/a</span></span>                                                          |
| <span data-ttu-id="0ad70-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ad70-117">Application</span></span>                            | <span data-ttu-id="0ad70-118">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0ad70-118">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ad70-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ad70-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="0ad70-120">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ad70-120">Request body</span></span>

<span data-ttu-id="0ad70-121">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="0ad70-121">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="0ad70-122">Пример</span><span class="sxs-lookup"><span data-stu-id="0ad70-122">Example</span></span>

<span data-ttu-id="0ad70-123">В этом примере восстанавливается версия ресурса listItem, указанная пр `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="0ad70-123">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="0ad70-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ad70-124">Response</span></span>

<span data-ttu-id="0ad70-125">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="0ad70-125">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": []
}
-->


