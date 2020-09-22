---
title: Тип ресурса termsAndConditions
description: Объект termsAndConditions представляет метаданные и содержимое определенной политики условий. Содержимое политик условий предоставляется пользователю при первой попытке регистрации в Intune, а после этого — при правках, которые нужно повторно принять по требованию администратора. Благодаря им администраторы могут огласить условия, с которыми должен согласиться пользователь для регистрации устройств в Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de0999a449c8f92cb026743c344ec2cdbc82ab57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088624"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="a7815-105">Тип ресурса termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a7815-105">termsAndConditions resource type</span></span>

<span data-ttu-id="a7815-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7815-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7815-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7815-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7815-108">Объект termsAndConditions представляет метаданные и содержимое определенной политики условий.</span><span class="sxs-lookup"><span data-stu-id="a7815-108">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="a7815-109">Содержимое политик условий предоставляется пользователю при первой попытке регистрации в Intune, а после этого — при правках, которые нужно повторно принять по требованию администратора.</span><span class="sxs-lookup"><span data-stu-id="a7815-109">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="a7815-110">Благодаря им администраторы могут огласить условия, с которыми должен согласиться пользователь для регистрации устройств в Intune.</span><span class="sxs-lookup"><span data-stu-id="a7815-110">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="a7815-111">Методы</span><span class="sxs-lookup"><span data-stu-id="a7815-111">Methods</span></span>
|<span data-ttu-id="a7815-112">Метод</span><span class="sxs-lookup"><span data-stu-id="a7815-112">Method</span></span>|<span data-ttu-id="a7815-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a7815-113">Return Type</span></span>|<span data-ttu-id="a7815-114">Описание</span><span class="sxs-lookup"><span data-stu-id="a7815-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7815-115">Список termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a7815-115">List termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="a7815-116">Коллекция объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)</span><span class="sxs-lookup"><span data-stu-id="a7815-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="a7815-117">Список свойств и связей объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="a7815-117">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="a7815-118">Получение объекта termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a7815-118">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="a7815-119">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a7815-119">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="a7815-120">Чтение свойств и связей объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="a7815-120">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="a7815-121">Создание объекта termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a7815-121">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="a7815-122">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a7815-122">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="a7815-123">Создание объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="a7815-123">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="a7815-124">Удаление объекта termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a7815-124">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="a7815-125">Нет</span><span class="sxs-lookup"><span data-stu-id="a7815-125">None</span></span>|<span data-ttu-id="a7815-126">Удаление объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="a7815-126">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="a7815-127">Обновление объекта termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a7815-127">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="a7815-128">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a7815-128">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="a7815-129">Обновление свойств объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="a7815-129">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7815-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7815-130">Properties</span></span>
|<span data-ttu-id="a7815-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7815-131">Property</span></span>|<span data-ttu-id="a7815-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a7815-132">Type</span></span>|<span data-ttu-id="a7815-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a7815-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7815-134">id</span><span class="sxs-lookup"><span data-stu-id="a7815-134">id</span></span>|<span data-ttu-id="a7815-135">Строка</span><span class="sxs-lookup"><span data-stu-id="a7815-135">String</span></span>|<span data-ttu-id="a7815-136">Уникальный идентификатор политики использования.</span><span class="sxs-lookup"><span data-stu-id="a7815-136">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="a7815-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7815-137">createdDateTime</span></span>|<span data-ttu-id="a7815-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7815-138">DateTimeOffset</span></span>|<span data-ttu-id="a7815-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a7815-139">DateTime the object was created.</span></span>|
|<span data-ttu-id="a7815-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7815-140">lastModifiedDateTime</span></span>|<span data-ttu-id="a7815-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7815-141">DateTimeOffset</span></span>|<span data-ttu-id="a7815-142">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a7815-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a7815-143">displayName</span><span class="sxs-lookup"><span data-stu-id="a7815-143">displayName</span></span>|<span data-ttu-id="a7815-144">Строка</span><span class="sxs-lookup"><span data-stu-id="a7815-144">String</span></span>|<span data-ttu-id="a7815-145">Имя политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="a7815-145">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="a7815-146">description</span><span class="sxs-lookup"><span data-stu-id="a7815-146">description</span></span>|<span data-ttu-id="a7815-147">Строка</span><span class="sxs-lookup"><span data-stu-id="a7815-147">String</span></span>|<span data-ttu-id="a7815-148">Описание политики использования, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="a7815-148">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="a7815-149">title</span><span class="sxs-lookup"><span data-stu-id="a7815-149">title</span></span>|<span data-ttu-id="a7815-150">Строка</span><span class="sxs-lookup"><span data-stu-id="a7815-150">String</span></span>|<span data-ttu-id="a7815-151">Название условий, указанное администратором.</span><span class="sxs-lookup"><span data-stu-id="a7815-151">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="a7815-152">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="a7815-152">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="a7815-153">bodyText</span><span class="sxs-lookup"><span data-stu-id="a7815-153">bodyText</span></span>|<span data-ttu-id="a7815-154">String</span><span class="sxs-lookup"><span data-stu-id="a7815-154">String</span></span>|<span data-ttu-id="a7815-155">Основной текст условий, заданный администратором (как правило, сами условия).</span><span class="sxs-lookup"><span data-stu-id="a7815-155">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="a7815-156">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="a7815-156">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="a7815-157">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="a7815-157">acceptanceStatement</span></span>|<span data-ttu-id="a7815-158">String</span><span class="sxs-lookup"><span data-stu-id="a7815-158">String</span></span>|<span data-ttu-id="a7815-159">Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике.</span><span class="sxs-lookup"><span data-stu-id="a7815-159">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="a7815-160">Показывается пользователю при запросе на принятие политики использования.</span><span class="sxs-lookup"><span data-stu-id="a7815-160">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="a7815-161">version</span><span class="sxs-lookup"><span data-stu-id="a7815-161">version</span></span>|<span data-ttu-id="a7815-162">Int32</span><span class="sxs-lookup"><span data-stu-id="a7815-162">Int32</span></span>|<span data-ttu-id="a7815-163">Целое число, указывающее текущую версию условий.</span><span class="sxs-lookup"><span data-stu-id="a7815-163">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="a7815-164">Увеличивается, когда администратор вносит изменения в условия и запрашивает повторное принятие измененной политики у пользователей.</span><span class="sxs-lookup"><span data-stu-id="a7815-164">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7815-165">Связи</span><span class="sxs-lookup"><span data-stu-id="a7815-165">Relationships</span></span>
|<span data-ttu-id="a7815-166">Связь</span><span class="sxs-lookup"><span data-stu-id="a7815-166">Relationship</span></span>|<span data-ttu-id="a7815-167">Тип</span><span class="sxs-lookup"><span data-stu-id="a7815-167">Type</span></span>|<span data-ttu-id="a7815-168">Описание</span><span class="sxs-lookup"><span data-stu-id="a7815-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7815-169">assignments</span><span class="sxs-lookup"><span data-stu-id="a7815-169">assignments</span></span>|<span data-ttu-id="a7815-170">Коллекция объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a7815-170">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="a7815-171">Список назначений для этой политики условий.</span><span class="sxs-lookup"><span data-stu-id="a7815-171">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="a7815-172">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="a7815-172">acceptanceStatuses</span></span>|<span data-ttu-id="a7815-173">Коллекция объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="a7815-173">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="a7815-174">Список состояний принятия для этой политики условий.</span><span class="sxs-lookup"><span data-stu-id="a7815-174">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7815-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7815-175">JSON Representation</span></span>
<span data-ttu-id="a7815-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7815-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```









