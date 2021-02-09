---
title: Тип ресурса custodian
description: В контексте eDiscovery представляет пользователя и все его цифровые активы, такие как электронная почта и документы.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 6c6b2befbb4066b851e38e6e17fd8be5aa59b031
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157696"
---
# <a name="custodian-resource-type"></a><span data-ttu-id="96a63-103">Тип ресурса custodian</span><span class="sxs-lookup"><span data-stu-id="96a63-103">custodian resource type</span></span>

<span data-ttu-id="96a63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96a63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96a63-105">В контексте eDiscovery представляет пользователя и все его цифровые активы, такие как электронная почта и документы.</span><span class="sxs-lookup"><span data-stu-id="96a63-105">In the context of eDiscovery, represents a user and all of their digital assets, such as email and documents.</span></span>

## <a name="methods"></a><span data-ttu-id="96a63-106">Методы</span><span class="sxs-lookup"><span data-stu-id="96a63-106">Methods</span></span>

|<span data-ttu-id="96a63-107">Метод</span><span class="sxs-lookup"><span data-stu-id="96a63-107">Method</span></span>|<span data-ttu-id="96a63-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="96a63-108">Return type</span></span>|<span data-ttu-id="96a63-109">Описание</span><span class="sxs-lookup"><span data-stu-id="96a63-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96a63-110">Список хранителей</span><span class="sxs-lookup"><span data-stu-id="96a63-110">List custodians</span></span>](../api/ediscoverycase-list-custodians.md)|<span data-ttu-id="96a63-111">[коллекция custodian](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="96a63-111">[custodian](../resources/custodian.md) collection</span></span>|<span data-ttu-id="96a63-112">Получите список объектов **хранителя** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="96a63-112">Get a list of **custodian** objects and their properties.</span></span>|
|[<span data-ttu-id="96a63-113">Создание хранителя</span><span class="sxs-lookup"><span data-stu-id="96a63-113">Create custodian</span></span>](../api/ediscoverycase-post-custodians.md)|[<span data-ttu-id="96a63-114">custodian</span><span class="sxs-lookup"><span data-stu-id="96a63-114">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="96a63-115">Создание объекта **хранителя.**</span><span class="sxs-lookup"><span data-stu-id="96a63-115">Create a new **custodian** object.</span></span>|
|[<span data-ttu-id="96a63-116">Получить хранителя</span><span class="sxs-lookup"><span data-stu-id="96a63-116">Get custodian</span></span>](../api/custodian-get.md)|[<span data-ttu-id="96a63-117">custodian</span><span class="sxs-lookup"><span data-stu-id="96a63-117">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="96a63-118">Чтение свойств и связей объекта **хранителя.**</span><span class="sxs-lookup"><span data-stu-id="96a63-118">Read the properties and relationships of a **custodian** object.</span></span>|
|[<span data-ttu-id="96a63-119">Обновление хранителя</span><span class="sxs-lookup"><span data-stu-id="96a63-119">Update custodian</span></span>](../api/custodian-update.md)|[<span data-ttu-id="96a63-120">custodian</span><span class="sxs-lookup"><span data-stu-id="96a63-120">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="96a63-121">Обновление свойств объекта **custodian.**</span><span class="sxs-lookup"><span data-stu-id="96a63-121">Update the properties of a **custodian** object.</span></span>|
|[<span data-ttu-id="96a63-122">release</span><span class="sxs-lookup"><span data-stu-id="96a63-122">release</span></span>](../api/custodian-release.md)|<span data-ttu-id="96a63-123">Нет</span><span class="sxs-lookup"><span data-stu-id="96a63-123">None</span></span>|<span data-ttu-id="96a63-124">Освобождение хранителя из дела.</span><span class="sxs-lookup"><span data-stu-id="96a63-124">Release a custodian from a case.</span></span>|
|[<span data-ttu-id="96a63-125">activate</span><span class="sxs-lookup"><span data-stu-id="96a63-125">activate</span></span>](../api/custodian-activate.md)|<span data-ttu-id="96a63-126">Нет</span><span class="sxs-lookup"><span data-stu-id="96a63-126">None</span></span>|<span data-ttu-id="96a63-127">Повторно активировать хранителя, освобожденного из дела, и снова сделать его частью дела.</span><span class="sxs-lookup"><span data-stu-id="96a63-127">Reactivate a custodian that has been released from a case and make them part of the case again.</span></span>|
|[<span data-ttu-id="96a63-128">Список siteSources</span><span class="sxs-lookup"><span data-stu-id="96a63-128">List siteSources</span></span>](../api/custodian-list-sitesources.md)|<span data-ttu-id="96a63-129">[Коллекция siteSource](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="96a63-129">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="96a63-130">Получите ресурсы **siteSource** из свойства навигации **siteSources.**</span><span class="sxs-lookup"><span data-stu-id="96a63-130">Get the **siteSource** resources from the **siteSources** navigation property.</span></span>|
|[<span data-ttu-id="96a63-131">Создание siteSources</span><span class="sxs-lookup"><span data-stu-id="96a63-131">Create siteSources</span></span>](../api/custodian-post-sitesources.md)|[<span data-ttu-id="96a63-132">siteSource</span><span class="sxs-lookup"><span data-stu-id="96a63-132">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="96a63-133">Создание объекта **siteSource.**</span><span class="sxs-lookup"><span data-stu-id="96a63-133">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="96a63-134">Список unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="96a63-134">List unifiedGroupSources</span></span>](../api/custodian-list-unifiedgroupsources.md)|<span data-ttu-id="96a63-135">[Коллекция unifiedGroupSource](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="96a63-135">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="96a63-136">Получите ресурсы **unifiedGroupSource из** свойства навигации **unifiedGroupSources.**</span><span class="sxs-lookup"><span data-stu-id="96a63-136">Get the **unifiedGroupSource** resources from the **unifiedGroupSources** navigation property.</span></span>|
|[<span data-ttu-id="96a63-137">Создание unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="96a63-137">Create unifiedGroupSources</span></span>](../api/custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="96a63-138">unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="96a63-138">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="96a63-139">Создание объекта **unifiedGroupSource.**</span><span class="sxs-lookup"><span data-stu-id="96a63-139">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="96a63-140">Список userSources</span><span class="sxs-lookup"><span data-stu-id="96a63-140">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="96a63-141">[Коллекция userSource](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="96a63-141">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="96a63-142">Получите ресурсы **userSource** из свойства **навигации userSources.**</span><span class="sxs-lookup"><span data-stu-id="96a63-142">Get the **userSource** resources from the **userSources** navigation property.</span></span>|
|[<span data-ttu-id="96a63-143">Создание userSources</span><span class="sxs-lookup"><span data-stu-id="96a63-143">Create userSources</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="96a63-144">userSource</span><span class="sxs-lookup"><span data-stu-id="96a63-144">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="96a63-145">Создание объекта **userSource.**</span><span class="sxs-lookup"><span data-stu-id="96a63-145">Create a new **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96a63-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="96a63-146">Properties</span></span>

|<span data-ttu-id="96a63-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="96a63-147">Property</span></span>|<span data-ttu-id="96a63-148">Тип</span><span class="sxs-lookup"><span data-stu-id="96a63-148">Type</span></span>|<span data-ttu-id="96a63-149">Описание</span><span class="sxs-lookup"><span data-stu-id="96a63-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96a63-150">acknowledgedDateTime</span><span class="sxs-lookup"><span data-stu-id="96a63-150">acknowledgedDateTime</span></span>|<span data-ttu-id="96a63-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96a63-151">DateTimeOffset</span></span>|<span data-ttu-id="96a63-152">Дата и время, когда хранител подтвердил уведомление об удержании.</span><span class="sxs-lookup"><span data-stu-id="96a63-152">Date and time the custodian acknowledged a hold notification.</span></span>|
|<span data-ttu-id="96a63-153">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="96a63-153">applyHoldToSources</span></span>|<span data-ttu-id="96a63-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="96a63-154">Boolean</span></span>|<span data-ttu-id="96a63-155">Определяет, были ли источники хранителя помещены на удержание во время создания.</span><span class="sxs-lookup"><span data-stu-id="96a63-155">Identifies whether a custodian's sources were placed on hold during creation.</span></span>|
|<span data-ttu-id="96a63-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96a63-156">createdDateTime</span></span>|<span data-ttu-id="96a63-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96a63-157">DateTimeOffset</span></span>|<span data-ttu-id="96a63-158">Дата и время, когда хранители были добавлены в дело.</span><span class="sxs-lookup"><span data-stu-id="96a63-158">Date and time when the custodian was added to the case.</span></span>|
|<span data-ttu-id="96a63-159">displayName</span><span class="sxs-lookup"><span data-stu-id="96a63-159">displayName</span></span>|<span data-ttu-id="96a63-160">String</span><span class="sxs-lookup"><span data-stu-id="96a63-160">String</span></span>|<span data-ttu-id="96a63-161">Отображаемого имени хранителя.</span><span class="sxs-lookup"><span data-stu-id="96a63-161">Display name of the custodian.</span></span>|
|<span data-ttu-id="96a63-162">email</span><span class="sxs-lookup"><span data-stu-id="96a63-162">email</span></span>|<span data-ttu-id="96a63-163">String</span><span class="sxs-lookup"><span data-stu-id="96a63-163">String</span></span>|<span data-ttu-id="96a63-164">Адрес электронной почты хранителя.</span><span class="sxs-lookup"><span data-stu-id="96a63-164">Email address of the custodian.</span></span>|
|<span data-ttu-id="96a63-165">id</span><span class="sxs-lookup"><span data-stu-id="96a63-165">id</span></span>|<span data-ttu-id="96a63-166">String</span><span class="sxs-lookup"><span data-stu-id="96a63-166">String</span></span>|<span data-ttu-id="96a63-167">ИД хранителя в указанном случае.</span><span class="sxs-lookup"><span data-stu-id="96a63-167">The ID for the custodian in the specified case.</span></span> <span data-ttu-id="96a63-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96a63-168">Read-only.</span></span>|
|<span data-ttu-id="96a63-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96a63-169">lastModifiedDateTime</span></span>|<span data-ttu-id="96a63-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96a63-170">DateTimeOffset</span></span>|<span data-ttu-id="96a63-171">Дата и время последнего изменения объекта хранителя</span><span class="sxs-lookup"><span data-stu-id="96a63-171">Date and time the custodian object was last modified</span></span>|
|<span data-ttu-id="96a63-172">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="96a63-172">releasedDateTime</span></span>|<span data-ttu-id="96a63-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96a63-173">DateTimeOffset</span></span>|<span data-ttu-id="96a63-174">Дата и время освобождения хранителя из дела.</span><span class="sxs-lookup"><span data-stu-id="96a63-174">Date and time the custodian was released from the case.</span></span>|
|<span data-ttu-id="96a63-175">status</span><span class="sxs-lookup"><span data-stu-id="96a63-175">status</span></span>|<span data-ttu-id="96a63-176">custodianStatus</span><span class="sxs-lookup"><span data-stu-id="96a63-176">custodianStatus</span></span>|<span data-ttu-id="96a63-177">Состояние хранителя.</span><span class="sxs-lookup"><span data-stu-id="96a63-177">Status of the custodian.</span></span> <span data-ttu-id="96a63-178">Возможные значения: `active`, `released`.</span><span class="sxs-lookup"><span data-stu-id="96a63-178">Possible values are: `active`, `released`.</span></span>|

### <a name="custodianstatus-values"></a><span data-ttu-id="96a63-179">значения custodianStatus</span><span class="sxs-lookup"><span data-stu-id="96a63-179">custodianStatus values</span></span>

|<span data-ttu-id="96a63-180">Member</span><span class="sxs-lookup"><span data-stu-id="96a63-180">Member</span></span>|<span data-ttu-id="96a63-181">Описание</span><span class="sxs-lookup"><span data-stu-id="96a63-181">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="96a63-182">active</span><span class="sxs-lookup"><span data-stu-id="96a63-182">active</span></span>|<span data-ttu-id="96a63-183">Хранителя является активной частью дела.</span><span class="sxs-lookup"><span data-stu-id="96a63-183">Custodian is an active part of the case.</span></span> |
|<span data-ttu-id="96a63-184">released</span><span class="sxs-lookup"><span data-stu-id="96a63-184">released</span></span>|<span data-ttu-id="96a63-185">Хранители освобождены из дела.</span><span class="sxs-lookup"><span data-stu-id="96a63-185">Custodian is released from the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96a63-186">Связи</span><span class="sxs-lookup"><span data-stu-id="96a63-186">Relationships</span></span>

|<span data-ttu-id="96a63-187">Связь</span><span class="sxs-lookup"><span data-stu-id="96a63-187">Relationship</span></span>|<span data-ttu-id="96a63-188">Тип</span><span class="sxs-lookup"><span data-stu-id="96a63-188">Type</span></span>|<span data-ttu-id="96a63-189">Описание</span><span class="sxs-lookup"><span data-stu-id="96a63-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96a63-190">siteSources</span><span class="sxs-lookup"><span data-stu-id="96a63-190">siteSources</span></span>|<span data-ttu-id="96a63-191">[Коллекция siteSource](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="96a63-191">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="96a63-192">Объект источника данных для сайтов SharePoint, связанных с хранителями.</span><span class="sxs-lookup"><span data-stu-id="96a63-192">Data source entity for SharePoint sites associated with the custodian.</span></span>|
|<span data-ttu-id="96a63-193">unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="96a63-193">unifiedGroupSources</span></span>|<span data-ttu-id="96a63-194">[Коллекция unifiedGroupSource](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="96a63-194">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="96a63-195">Объект источника данных для групп, связанных с хранителями.</span><span class="sxs-lookup"><span data-stu-id="96a63-195">Data source entity for groups associated with the custodian.</span></span>|
|<span data-ttu-id="96a63-196">userSources</span><span class="sxs-lookup"><span data-stu-id="96a63-196">userSources</span></span>|<span data-ttu-id="96a63-197">[Коллекция userSource](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="96a63-197">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="96a63-198">Объект источника данных для хранителя.</span><span class="sxs-lookup"><span data-stu-id="96a63-198">Data source entity for a the custodian.</span></span> <span data-ttu-id="96a63-199">Это контейнер для почтового ящика хранителя и сайта OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="96a63-199">This is the container for a custodian's mailbox and OneDrive for Business site.</span></span>|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a><span data-ttu-id="96a63-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96a63-200">JSON representation</span></span>

<span data-ttu-id="96a63-201">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96a63-201">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.custodian",
  "email": "String",
  "applyHoldToSources": "Boolean",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "acknowledgedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String"
}
```
