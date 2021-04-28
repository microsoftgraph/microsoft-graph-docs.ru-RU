---
title: Список updatableAssets
description: Получите список объектов updatableAsset и их свойств.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: e5eebb39af41bd31ee0e2d68404480ea84cd51dc
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067627"
---
# <a name="list-updatableassets"></a><span data-ttu-id="9f7a0-103">Список updatableAssets</span><span class="sxs-lookup"><span data-stu-id="9f7a0-103">List updatableAssets</span></span>
<span data-ttu-id="9f7a0-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="9f7a0-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f7a0-105">Получите список [объектов updatableAsset](../resources/windowsupdates-updatableasset.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="9f7a0-105">Get a list of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects and their properties.</span></span>

<span data-ttu-id="9f7a0-106">Перечисление updatable assets возвращает **updatableAsset** ресурсы следующих производных типов: [azureADDevice](../resources/windowsupdates-azureADDevice.md) и [updatableAssetGroup.](../resources/windowsupdates-updatableassetGroup.md)</span><span class="sxs-lookup"><span data-stu-id="9f7a0-106">Listing updatable assets returns **updatableAsset** resources of the following derived types: [azureADDevice](../resources/windowsupdates-azureADDevice.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetGroup.md).</span></span>

<span data-ttu-id="9f7a0-107">Используйте [ресурсы azureADDevice](windowsupdates-updates-list-updatableassets-azureaddevice.md) списка или список [updatableAssetGroup для](windowsupdates-updates-list-updatableassets-updatableassetgroup.md) фильтрации и получения ресурсов только одного из производных типов.</span><span class="sxs-lookup"><span data-stu-id="9f7a0-107">Use [list azureADDevice resources](windowsupdates-updates-list-updatableassets-azureaddevice.md) or [list updatableAssetGroup resources](windowsupdates-updates-list-updatableassets-updatableassetgroup.md) to filter and get resources of only one of the derived types.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f7a0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f7a0-108">Permissions</span></span>
<span data-ttu-id="9f7a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f7a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f7a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f7a0-111">Permission type</span></span>|<span data-ttu-id="9f7a0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f7a0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f7a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f7a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f7a0-114">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f7a0-114">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="9f7a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f7a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f7a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f7a0-116">Not supported.</span></span>|
|<span data-ttu-id="9f7a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f7a0-117">Application</span></span>|<span data-ttu-id="9f7a0-118">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f7a0-118">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f7a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f7a0-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f7a0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f7a0-120">Optional query parameters</span></span>
<span data-ttu-id="9f7a0-121">Этот метод поддерживает некоторые параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="9f7a0-121">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="9f7a0-122">Чтобы использовать параметр запроса для свойства, которое не унаследовано от [updatableAsset,](../resources/windowsupdates-updatableasset.md)включайте полный тип ресурса для свойства.</span><span class="sxs-lookup"><span data-stu-id="9f7a0-122">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="9f7a0-123">Например, чтобы применить `$select` к свойству **ошибок** [azureADDevice,](../resources/windowsupdates-azureaddevice.md)используйте `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="9f7a0-123">For example, to apply `$select` on the **errors** property of [azureADDevice](../resources/windowsupdates-azureaddevice.md), use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f7a0-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f7a0-124">Request headers</span></span>
|<span data-ttu-id="9f7a0-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9f7a0-125">Name</span></span>|<span data-ttu-id="9f7a0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9f7a0-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f7a0-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f7a0-127">Authorization</span></span>|<span data-ttu-id="9f7a0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f7a0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f7a0-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f7a0-130">Request body</span></span>
<span data-ttu-id="9f7a0-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f7a0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f7a0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f7a0-132">Response</span></span>

<span data-ttu-id="9f7a0-133">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [updatableAsset](../resources/windowsupdates-updatableasset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9f7a0-133">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f7a0-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="9f7a0-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f7a0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f7a0-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets
```


### <a name="response"></a><span data-ttu-id="9f7a0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f7a0-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
      "errors": [],
      "enrollments": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
          "updateCategory": "feature"
        }
      ]
    }
  ]
}
```

