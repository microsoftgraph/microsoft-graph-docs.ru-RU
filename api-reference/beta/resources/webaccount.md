---
title: Тип ресурса "учетная запись"
description: Тип ресурса "учетная запись"
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 29d66809d14cfc72d43286aef801490cef20cb9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057684"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="50fe9-103">Тип ресурса "учетная запись"</span><span class="sxs-lookup"><span data-stu-id="50fe9-103">webAccount resource type</span></span>

<span data-ttu-id="50fe9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50fe9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50fe9-105">Представляет веб-учетные записи, которые пользователь указал, используют или добавили в свой [профиль](profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="50fe9-105">Represents web accounts the user has indicated they use or have added to their user [profile](profile.md).</span></span>

<span data-ttu-id="50fe9-106">Этот тип ресурса наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="50fe9-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="50fe9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="50fe9-107">Methods</span></span>

|<span data-ttu-id="50fe9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="50fe9-108">Method</span></span>|<span data-ttu-id="50fe9-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="50fe9-109">Return type</span></span>|<span data-ttu-id="50fe9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="50fe9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50fe9-111">Список учетных записей</span><span class="sxs-lookup"><span data-stu-id="50fe9-111">List webAccounts</span></span>](../api/profile-list-webaccounts.md)|<span data-ttu-id="50fe9-112">Коллекция [учетных записей](../resources/webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="50fe9-112">[webAccount](../resources/webaccount.md) collection</span></span>|<span data-ttu-id="50fe9-113">Получение ресурсов учетной записи службы из свойства навигации для учетных записей учетных записей.</span><span class="sxs-lookup"><span data-stu-id="50fe9-113">Get the webAccount resources from the webAccounts navigation property.</span></span>|
|[<span data-ttu-id="50fe9-114">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="50fe9-114">Create webAccount</span></span>](../api/profile-post-webaccounts.md)|[<span data-ttu-id="50fe9-115">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="50fe9-115">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="50fe9-116">Создайте новый объект учетной записи.</span><span class="sxs-lookup"><span data-stu-id="50fe9-116">Create a new webAccount object.</span></span>|
|[<span data-ttu-id="50fe9-117">Получение учетной записи службы</span><span class="sxs-lookup"><span data-stu-id="50fe9-117">Get webAccount</span></span>](../api/webaccount-get.md)|[<span data-ttu-id="50fe9-118">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="50fe9-118">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="50fe9-119">Чтение свойств и связей объекта веб- [учетных записей](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="50fe9-119">Read the properties and relationships of a [webAccount](../resources/webaccount.md) object.</span></span>|
|[<span data-ttu-id="50fe9-120">Обновление учетной записи</span><span class="sxs-lookup"><span data-stu-id="50fe9-120">Update webAccount</span></span>](../api/webaccount-update.md)|[<span data-ttu-id="50fe9-121">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="50fe9-121">webAccount</span></span>](../resources/webaccount.md)|<span data-ttu-id="50fe9-122">Обновление свойств объекта [учетной записи](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="50fe9-122">Update the properties of a [webAccount](../resources/webaccount.md) object.</span></span>|
|[<span data-ttu-id="50fe9-123">Удаление учетной записи службы</span><span class="sxs-lookup"><span data-stu-id="50fe9-123">Delete webAccount</span></span>](../api/webaccount-delete.md)|<span data-ttu-id="50fe9-124">Нет</span><span class="sxs-lookup"><span data-stu-id="50fe9-124">None</span></span>|<span data-ttu-id="50fe9-125">Удаляет объект [учетной записи](../resources/webaccount.md) .</span><span class="sxs-lookup"><span data-stu-id="50fe9-125">Deletes a [webAccount](../resources/webaccount.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50fe9-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="50fe9-126">Properties</span></span>

|<span data-ttu-id="50fe9-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="50fe9-127">Property</span></span>|<span data-ttu-id="50fe9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="50fe9-128">Type</span></span>|<span data-ttu-id="50fe9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="50fe9-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50fe9-130">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="50fe9-130">allowedAudiences</span></span>|<span data-ttu-id="50fe9-131">String</span><span class="sxs-lookup"><span data-stu-id="50fe9-131">String</span></span>|<span data-ttu-id="50fe9-132">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="50fe9-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="50fe9-133">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="50fe9-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="50fe9-134">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="50fe9-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="50fe9-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="50fe9-135">createdBy</span></span>|[<span data-ttu-id="50fe9-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="50fe9-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="50fe9-137">Предоставляет идентификатор пользователя и/или приложения, создавшего сущность.</span><span class="sxs-lookup"><span data-stu-id="50fe9-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="50fe9-138">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="50fe9-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="50fe9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50fe9-139">createdDateTime</span></span>|<span data-ttu-id="50fe9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50fe9-140">DateTimeOffset</span></span>|<span data-ttu-id="50fe9-141">Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.</span><span class="sxs-lookup"><span data-stu-id="50fe9-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="50fe9-142">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="50fe9-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="50fe9-143">description</span><span class="sxs-lookup"><span data-stu-id="50fe9-143">description</span></span>|<span data-ttu-id="50fe9-144">String</span><span class="sxs-lookup"><span data-stu-id="50fe9-144">String</span></span>|<span data-ttu-id="50fe9-145">Содержит описание, предоставленное пользователем для учетной записи службы, на которую выполняется ссылка.</span><span class="sxs-lookup"><span data-stu-id="50fe9-145">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="50fe9-146">id</span><span class="sxs-lookup"><span data-stu-id="50fe9-146">id</span></span>|<span data-ttu-id="50fe9-147">String</span><span class="sxs-lookup"><span data-stu-id="50fe9-147">String</span></span>|<span data-ttu-id="50fe9-148">Идентификатор, используемый для индивидуальной адресации объекта.</span><span class="sxs-lookup"><span data-stu-id="50fe9-148">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="50fe9-149">Наследуется от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="50fe9-149">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="50fe9-150">выводов</span><span class="sxs-lookup"><span data-stu-id="50fe9-150">inference</span></span>|[<span data-ttu-id="50fe9-151">инференцедата</span><span class="sxs-lookup"><span data-stu-id="50fe9-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="50fe9-152">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="50fe9-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="50fe9-153">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="50fe9-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="50fe9-154">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="50fe9-154">lastModifiedBy</span></span>|[<span data-ttu-id="50fe9-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="50fe9-155">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="50fe9-156">Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект.</span><span class="sxs-lookup"><span data-stu-id="50fe9-156">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="50fe9-157">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="50fe9-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="50fe9-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50fe9-158">lastModifiedDateTime</span></span>|<span data-ttu-id="50fe9-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50fe9-159">DateTimeOffset</span></span>|<span data-ttu-id="50fe9-160">Предоставляет значение dateTimeOffset для объекта, когда была создана сущность.</span><span class="sxs-lookup"><span data-stu-id="50fe9-160">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="50fe9-161">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="50fe9-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="50fe9-162">service</span><span class="sxs-lookup"><span data-stu-id="50fe9-162">service</span></span>|[<span data-ttu-id="50fe9-163">сервицеинформатион</span><span class="sxs-lookup"><span data-stu-id="50fe9-163">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="50fe9-164">Содержит основные сведения о связанной службе.</span><span class="sxs-lookup"><span data-stu-id="50fe9-164">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="50fe9-165">source</span><span class="sxs-lookup"><span data-stu-id="50fe9-165">source</span></span>|[<span data-ttu-id="50fe9-166">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="50fe9-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="50fe9-167">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="50fe9-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="50fe9-168">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="50fe9-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="50fe9-169">статусмессаже</span><span class="sxs-lookup"><span data-stu-id="50fe9-169">statusMessage</span></span>|<span data-ttu-id="50fe9-170">String</span><span class="sxs-lookup"><span data-stu-id="50fe9-170">String</span></span>|<span data-ttu-id="50fe9-171">Содержит сообщение о состоянии от облачной службы, если оно предоставлено или синхронизировано.</span><span class="sxs-lookup"><span data-stu-id="50fe9-171">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="50fe9-172">userId</span><span class="sxs-lookup"><span data-stu-id="50fe9-172">userId</span></span>|<span data-ttu-id="50fe9-173">String</span><span class="sxs-lookup"><span data-stu-id="50fe9-173">String</span></span>|<span data-ttu-id="50fe9-174">Имя пользователя, отображаемое для учетной записи Account.</span><span class="sxs-lookup"><span data-stu-id="50fe9-174">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="50fe9-175">webUrl</span><span class="sxs-lookup"><span data-stu-id="50fe9-175">webUrl</span></span>|<span data-ttu-id="50fe9-176">String</span><span class="sxs-lookup"><span data-stu-id="50fe9-176">String</span></span>|<span data-ttu-id="50fe9-177">Содержит ссылку на профиль пользователя в облачной службе, если она существует.</span><span class="sxs-lookup"><span data-stu-id="50fe9-177">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50fe9-178">Связи</span><span class="sxs-lookup"><span data-stu-id="50fe9-178">Relationships</span></span>
<span data-ttu-id="50fe9-179">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="50fe9-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50fe9-180">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="50fe9-180">JSON representation</span></span>
<span data-ttu-id="50fe9-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50fe9-181">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.webAccount",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "description": "String",
  "userId": "String",
  "service": {
    "@odata.type": "microsoft.graph.serviceInformation"
  },
  "statusMessage": "String",
  "webUrl": "String"
}
```


