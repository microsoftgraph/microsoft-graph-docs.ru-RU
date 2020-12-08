---
title: Тип ресурса хранитель
description: В контексте обнаружения электронных данных представляет пользователя и все свои цифровые ресурсы, такие как электронная почта и документы.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: a2e22f711eaec4cd68cc5026e36b900d5284e71a
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597831"
---
# <a name="custodian-resource-type"></a><span data-ttu-id="22ef9-103">Тип ресурса хранитель</span><span class="sxs-lookup"><span data-stu-id="22ef9-103">custodian resource type</span></span>

<span data-ttu-id="22ef9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22ef9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22ef9-105">В контексте обнаружения электронных данных представляет пользователя и все свои цифровые ресурсы, такие как электронная почта и документы.</span><span class="sxs-lookup"><span data-stu-id="22ef9-105">In the context of eDiscovery, represents a user and all of their digital assets, such as email and documents.</span></span>

## <a name="methods"></a><span data-ttu-id="22ef9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="22ef9-106">Methods</span></span>

|<span data-ttu-id="22ef9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="22ef9-107">Method</span></span>|<span data-ttu-id="22ef9-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="22ef9-108">Return type</span></span>|<span data-ttu-id="22ef9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="22ef9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22ef9-110">Список custodians</span><span class="sxs-lookup"><span data-stu-id="22ef9-110">List custodians</span></span>](../api/ediscoverycase-list-custodians.md)|<span data-ttu-id="22ef9-111">Коллекция [хранитель](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="22ef9-111">[custodian](../resources/custodian.md) collection</span></span>|<span data-ttu-id="22ef9-112">Получение списка объектов **хранитель** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="22ef9-112">Get a list of **custodian** objects and their properties.</span></span>|
|[<span data-ttu-id="22ef9-113">Создание хранитель</span><span class="sxs-lookup"><span data-stu-id="22ef9-113">Create custodian</span></span>](../api/ediscoverycase-post-custodians.md)|[<span data-ttu-id="22ef9-114">Хранитель</span><span class="sxs-lookup"><span data-stu-id="22ef9-114">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="22ef9-115">Создание нового объекта **хранитель** .</span><span class="sxs-lookup"><span data-stu-id="22ef9-115">Create a new **custodian** object.</span></span>|
|[<span data-ttu-id="22ef9-116">Получение хранитель</span><span class="sxs-lookup"><span data-stu-id="22ef9-116">Get custodian</span></span>](../api/custodian-get.md)|[<span data-ttu-id="22ef9-117">Хранитель</span><span class="sxs-lookup"><span data-stu-id="22ef9-117">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="22ef9-118">Чтение свойств и связей объекта **хранитель** .</span><span class="sxs-lookup"><span data-stu-id="22ef9-118">Read the properties and relationships of a **custodian** object.</span></span>|
|[<span data-ttu-id="22ef9-119">Обновление хранитель</span><span class="sxs-lookup"><span data-stu-id="22ef9-119">Update custodian</span></span>](../api/custodian-update.md)|[<span data-ttu-id="22ef9-120">Хранитель</span><span class="sxs-lookup"><span data-stu-id="22ef9-120">custodian</span></span>](../resources/custodian.md)|<span data-ttu-id="22ef9-121">Обновление свойств объекта **хранитель** .</span><span class="sxs-lookup"><span data-stu-id="22ef9-121">Update the properties of a **custodian** object.</span></span>|
|[<span data-ttu-id="22ef9-122">удаления</span><span class="sxs-lookup"><span data-stu-id="22ef9-122">release</span></span>](../api/custodian-release.md)|<span data-ttu-id="22ef9-123">Нет</span><span class="sxs-lookup"><span data-stu-id="22ef9-123">None</span></span>|<span data-ttu-id="22ef9-124">Освобождение хранитель от случая.</span><span class="sxs-lookup"><span data-stu-id="22ef9-124">Release a custodian from a case.</span></span>|
|[<span data-ttu-id="22ef9-125">отключить</span><span class="sxs-lookup"><span data-stu-id="22ef9-125">activate</span></span>](../api/custodian-activate.md)|<span data-ttu-id="22ef9-126">Нет</span><span class="sxs-lookup"><span data-stu-id="22ef9-126">None</span></span>|<span data-ttu-id="22ef9-127">Повторно активируйте хранитель, выпущенные из случая, и сделайте их частью этого случая.</span><span class="sxs-lookup"><span data-stu-id="22ef9-127">Reactivate a custodian that has been released from a case and make them part of the case again.</span></span>|
|[<span data-ttu-id="22ef9-128">Список Ситесаурцес</span><span class="sxs-lookup"><span data-stu-id="22ef9-128">List siteSources</span></span>](../api/custodian-list-sitesources.md)|<span data-ttu-id="22ef9-129">Коллекция [ситесаурце](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="22ef9-129">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="22ef9-130">Получение ресурсов **ситесаурце** из свойства навигации **ситесаурцес** .</span><span class="sxs-lookup"><span data-stu-id="22ef9-130">Get the **siteSource** resources from the **siteSources** navigation property.</span></span>|
|[<span data-ttu-id="22ef9-131">Создание Ситесаурцес</span><span class="sxs-lookup"><span data-stu-id="22ef9-131">Create siteSources</span></span>](../api/custodian-post-sitesources.md)|[<span data-ttu-id="22ef9-132">ситесаурце</span><span class="sxs-lookup"><span data-stu-id="22ef9-132">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="22ef9-133">Создание нового объекта **ситесаурце** .</span><span class="sxs-lookup"><span data-stu-id="22ef9-133">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="22ef9-134">Список Унифиедграупсаурцес</span><span class="sxs-lookup"><span data-stu-id="22ef9-134">List unifiedGroupSources</span></span>](../api/custodian-list-unifiedgroupsources.md)|<span data-ttu-id="22ef9-135">Коллекция [унифиедграупсаурце](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="22ef9-135">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="22ef9-136">Получение ресурсов **унифиедграупсаурце** из свойства навигации **унифиедграупсаурцес** .</span><span class="sxs-lookup"><span data-stu-id="22ef9-136">Get the **unifiedGroupSource** resources from the **unifiedGroupSources** navigation property.</span></span>|
|[<span data-ttu-id="22ef9-137">Создание Унифиедграупсаурцес</span><span class="sxs-lookup"><span data-stu-id="22ef9-137">Create unifiedGroupSources</span></span>](../api/custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="22ef9-138">унифиедграупсаурце</span><span class="sxs-lookup"><span data-stu-id="22ef9-138">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="22ef9-139">Создание нового объекта **унифиедграупсаурце** .</span><span class="sxs-lookup"><span data-stu-id="22ef9-139">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="22ef9-140">Список Усерсаурцес</span><span class="sxs-lookup"><span data-stu-id="22ef9-140">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="22ef9-141">Коллекция [усерсаурце](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="22ef9-141">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="22ef9-142">Получение ресурсов **усерсаурце** из свойства навигации **усерсаурцес** .</span><span class="sxs-lookup"><span data-stu-id="22ef9-142">Get the **userSource** resources from the **userSources** navigation property.</span></span>|
|[<span data-ttu-id="22ef9-143">Создание Усерсаурцес</span><span class="sxs-lookup"><span data-stu-id="22ef9-143">Create userSources</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="22ef9-144">усерсаурце</span><span class="sxs-lookup"><span data-stu-id="22ef9-144">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="22ef9-145">Создание нового объекта **усерсаурце** .</span><span class="sxs-lookup"><span data-stu-id="22ef9-145">Create a new **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="22ef9-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="22ef9-146">Properties</span></span>

|<span data-ttu-id="22ef9-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="22ef9-147">Property</span></span>|<span data-ttu-id="22ef9-148">Тип</span><span class="sxs-lookup"><span data-stu-id="22ef9-148">Type</span></span>|<span data-ttu-id="22ef9-149">Описание</span><span class="sxs-lookup"><span data-stu-id="22ef9-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22ef9-150">аккновледжеддатетиме</span><span class="sxs-lookup"><span data-stu-id="22ef9-150">acknowledgedDateTime</span></span>|<span data-ttu-id="22ef9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ef9-151">DateTimeOffset</span></span>|<span data-ttu-id="22ef9-152">Дата и время, когда хранитель подтвердил уведомление об удержании.</span><span class="sxs-lookup"><span data-stu-id="22ef9-152">Date and time the custodian acknowledged a hold notification.</span></span>|
|<span data-ttu-id="22ef9-153">апплихолдтосаурцес</span><span class="sxs-lookup"><span data-stu-id="22ef9-153">applyHoldToSources</span></span>|<span data-ttu-id="22ef9-154">Логический</span><span class="sxs-lookup"><span data-stu-id="22ef9-154">Boolean</span></span>|<span data-ttu-id="22ef9-155">Определяет, были ли источники хранитель сохранены во время создания.</span><span class="sxs-lookup"><span data-stu-id="22ef9-155">Identifies whether a custodian's sources were placed on hold during creation.</span></span>|
|<span data-ttu-id="22ef9-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22ef9-156">createdDateTime</span></span>|<span data-ttu-id="22ef9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ef9-157">DateTimeOffset</span></span>|<span data-ttu-id="22ef9-158">Дата и время добавления хранитель к обращению.</span><span class="sxs-lookup"><span data-stu-id="22ef9-158">Date and time when the custodian was added to the case.</span></span>|
|<span data-ttu-id="22ef9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="22ef9-159">displayName</span></span>|<span data-ttu-id="22ef9-160">String</span><span class="sxs-lookup"><span data-stu-id="22ef9-160">String</span></span>|<span data-ttu-id="22ef9-161">Отображаемое имя хранитель.</span><span class="sxs-lookup"><span data-stu-id="22ef9-161">Display name of the custodian.</span></span>|
|<span data-ttu-id="22ef9-162">email</span><span class="sxs-lookup"><span data-stu-id="22ef9-162">email</span></span>|<span data-ttu-id="22ef9-163">String</span><span class="sxs-lookup"><span data-stu-id="22ef9-163">String</span></span>|<span data-ttu-id="22ef9-164">Адрес электронной почты хранитель.</span><span class="sxs-lookup"><span data-stu-id="22ef9-164">Email address of the custodian.</span></span>|
|<span data-ttu-id="22ef9-165">id</span><span class="sxs-lookup"><span data-stu-id="22ef9-165">id</span></span>|<span data-ttu-id="22ef9-166">String</span><span class="sxs-lookup"><span data-stu-id="22ef9-166">String</span></span>|<span data-ttu-id="22ef9-167">Идентификатор хранитель в указанном случае.</span><span class="sxs-lookup"><span data-stu-id="22ef9-167">The ID for the custodian in the specified case.</span></span> <span data-ttu-id="22ef9-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="22ef9-168">Read-only.</span></span>|
|<span data-ttu-id="22ef9-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22ef9-169">lastModifiedDateTime</span></span>|<span data-ttu-id="22ef9-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ef9-170">DateTimeOffset</span></span>|<span data-ttu-id="22ef9-171">Дата и время последнего изменения объекта хранитель</span><span class="sxs-lookup"><span data-stu-id="22ef9-171">Date and time the custodian object was last modified</span></span>|
|<span data-ttu-id="22ef9-172">релеаседдатетиме</span><span class="sxs-lookup"><span data-stu-id="22ef9-172">releasedDateTime</span></span>|<span data-ttu-id="22ef9-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ef9-173">DateTimeOffset</span></span>|<span data-ttu-id="22ef9-174">Дата и время, когда хранитель был выпущен из дела.</span><span class="sxs-lookup"><span data-stu-id="22ef9-174">Date and time the custodian was released from the case.</span></span>|
|<span data-ttu-id="22ef9-175">status</span><span class="sxs-lookup"><span data-stu-id="22ef9-175">status</span></span>|<span data-ttu-id="22ef9-176">кустодианстатус</span><span class="sxs-lookup"><span data-stu-id="22ef9-176">custodianStatus</span></span>|<span data-ttu-id="22ef9-177">Состояние хранитель.</span><span class="sxs-lookup"><span data-stu-id="22ef9-177">Status of the custodian.</span></span> <span data-ttu-id="22ef9-178">Возможные значения: `active`, `released`.</span><span class="sxs-lookup"><span data-stu-id="22ef9-178">Possible values are: `active`, `released`.</span></span>|

### <a name="custodianstatus-values"></a><span data-ttu-id="22ef9-179">значения Кустодианстатус</span><span class="sxs-lookup"><span data-stu-id="22ef9-179">custodianStatus values</span></span>

|<span data-ttu-id="22ef9-180">Member</span><span class="sxs-lookup"><span data-stu-id="22ef9-180">Member</span></span>|<span data-ttu-id="22ef9-181">Описание</span><span class="sxs-lookup"><span data-stu-id="22ef9-181">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="22ef9-182">ASP</span><span class="sxs-lookup"><span data-stu-id="22ef9-182">active</span></span>|<span data-ttu-id="22ef9-183">Хранитель — это активная часть этого случая.</span><span class="sxs-lookup"><span data-stu-id="22ef9-183">Custodian is an active part of the case.</span></span> |
|<span data-ttu-id="22ef9-184">снят</span><span class="sxs-lookup"><span data-stu-id="22ef9-184">released</span></span>|<span data-ttu-id="22ef9-185">Хранитель выпущен из этого случая.</span><span class="sxs-lookup"><span data-stu-id="22ef9-185">Custodian is released from the case.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22ef9-186">Связи</span><span class="sxs-lookup"><span data-stu-id="22ef9-186">Relationships</span></span>

|<span data-ttu-id="22ef9-187">Связь</span><span class="sxs-lookup"><span data-stu-id="22ef9-187">Relationship</span></span>|<span data-ttu-id="22ef9-188">Тип</span><span class="sxs-lookup"><span data-stu-id="22ef9-188">Type</span></span>|<span data-ttu-id="22ef9-189">Описание</span><span class="sxs-lookup"><span data-stu-id="22ef9-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22ef9-190">ситесаурцес</span><span class="sxs-lookup"><span data-stu-id="22ef9-190">siteSources</span></span>|<span data-ttu-id="22ef9-191">Коллекция [ситесаурце](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="22ef9-191">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="22ef9-192">Объект источника данных для сайтов SharePoint, связанных с хранитель.</span><span class="sxs-lookup"><span data-stu-id="22ef9-192">Data source entity for SharePoint sites associated with the custodian.</span></span>|
|<span data-ttu-id="22ef9-193">унифиедграупсаурцес</span><span class="sxs-lookup"><span data-stu-id="22ef9-193">unifiedGroupSources</span></span>|<span data-ttu-id="22ef9-194">Коллекция [унифиедграупсаурце](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="22ef9-194">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="22ef9-195">Сущность источника данных для групп, связанных с хранитель.</span><span class="sxs-lookup"><span data-stu-id="22ef9-195">Data source entity for groups associated with the custodian.</span></span>|
|<span data-ttu-id="22ef9-196">усерсаурцес</span><span class="sxs-lookup"><span data-stu-id="22ef9-196">userSources</span></span>|<span data-ttu-id="22ef9-197">Коллекция [усерсаурце](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="22ef9-197">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="22ef9-198">Сущность источника данных для объекта хранитель.</span><span class="sxs-lookup"><span data-stu-id="22ef9-198">Data source entity for a the custodian.</span></span> <span data-ttu-id="22ef9-199">Это контейнер для почтового ящика хранитель и сайта OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="22ef9-199">This is the container for a custodian's mailbox and OneDrive for Business site.</span></span>|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a><span data-ttu-id="22ef9-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22ef9-200">JSON representation</span></span>

<span data-ttu-id="22ef9-201">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22ef9-201">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
  "baseType": "",
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
