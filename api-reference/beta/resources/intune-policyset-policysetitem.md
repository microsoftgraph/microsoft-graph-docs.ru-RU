---
title: Тип ресурса Полицисетитем
description: Класс, содержащий свойства, используемые для элемента "набор политик".
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2701686d9f2f162a6ec01dfb143c2d8652dd098a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422508"
---
# <a name="policysetitem-resource-type"></a><span data-ttu-id="349bb-103">Тип ресурса Полицисетитем</span><span class="sxs-lookup"><span data-stu-id="349bb-103">policySetItem resource type</span></span>

<span data-ttu-id="349bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="349bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="349bb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="349bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="349bb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="349bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="349bb-107">Класс, содержащий свойства, используемые для элемента "набор политик".</span><span class="sxs-lookup"><span data-stu-id="349bb-107">A class containing the properties used for PolicySet Item.</span></span>

## <a name="methods"></a><span data-ttu-id="349bb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="349bb-108">Methods</span></span>
|<span data-ttu-id="349bb-109">Метод</span><span class="sxs-lookup"><span data-stu-id="349bb-109">Method</span></span>|<span data-ttu-id="349bb-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="349bb-110">Return Type</span></span>|<span data-ttu-id="349bb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="349bb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="349bb-112">Список Полицисетитемс</span><span class="sxs-lookup"><span data-stu-id="349bb-112">List policySetItems</span></span>](../api/intune-policyset-policysetitem-list.md)|<span data-ttu-id="349bb-113">Коллекция [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="349bb-113">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="349bb-114">Список свойств и связей объектов [полицисетитем](../resources/intune-policyset-policysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="349bb-114">List properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) objects.</span></span>|
|[<span data-ttu-id="349bb-115">Получение Полицисетитем</span><span class="sxs-lookup"><span data-stu-id="349bb-115">Get policySetItem</span></span>](../api/intune-policyset-policysetitem-get.md)|[<span data-ttu-id="349bb-116">policySetItem</span><span class="sxs-lookup"><span data-stu-id="349bb-116">policySetItem</span></span>](../resources/intune-policyset-policysetitem.md)|<span data-ttu-id="349bb-117">Чтение свойств и связей объекта [полицисетитем](../resources/intune-policyset-policysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="349bb-117">Read properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="349bb-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="349bb-118">Properties</span></span>
|<span data-ttu-id="349bb-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="349bb-119">Property</span></span>|<span data-ttu-id="349bb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="349bb-120">Type</span></span>|<span data-ttu-id="349bb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="349bb-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="349bb-122">id</span><span class="sxs-lookup"><span data-stu-id="349bb-122">id</span></span>|<span data-ttu-id="349bb-123">String</span><span class="sxs-lookup"><span data-stu-id="349bb-123">String</span></span>|<span data-ttu-id="349bb-124">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="349bb-124">Key of the MobileAppPolicySetItem.</span></span>|
|<span data-ttu-id="349bb-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="349bb-125">createdDateTime</span></span>|<span data-ttu-id="349bb-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="349bb-126">DateTimeOffset</span></span>|<span data-ttu-id="349bb-127">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="349bb-127">Creation time of the PolicySetItem.</span></span>|
|<span data-ttu-id="349bb-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="349bb-128">lastModifiedDateTime</span></span>|<span data-ttu-id="349bb-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="349bb-129">DateTimeOffset</span></span>|<span data-ttu-id="349bb-130">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="349bb-130">Last modified time of the PolicySetItem.</span></span>|
|<span data-ttu-id="349bb-131">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="349bb-131">payloadId</span></span>|<span data-ttu-id="349bb-132">String</span><span class="sxs-lookup"><span data-stu-id="349bb-132">String</span></span>|<span data-ttu-id="349bb-133">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="349bb-133">PayloadId of the PolicySetItem.</span></span>|
|<span data-ttu-id="349bb-134">itemType</span><span class="sxs-lookup"><span data-stu-id="349bb-134">itemType</span></span>|<span data-ttu-id="349bb-135">String</span><span class="sxs-lookup"><span data-stu-id="349bb-135">String</span></span>|<span data-ttu-id="349bb-136">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="349bb-136">policySetType of the PolicySetItem.</span></span>|
|<span data-ttu-id="349bb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="349bb-137">displayName</span></span>|<span data-ttu-id="349bb-138">Строка</span><span class="sxs-lookup"><span data-stu-id="349bb-138">String</span></span>|<span data-ttu-id="349bb-139">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="349bb-139">DisplayName of the PolicySetItem.</span></span>|
|<span data-ttu-id="349bb-140">status</span><span class="sxs-lookup"><span data-stu-id="349bb-140">status</span></span>|[<span data-ttu-id="349bb-141">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="349bb-141">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="349bb-142">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="349bb-142">Status of the PolicySetItem.</span></span> <span data-ttu-id="349bb-143">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="349bb-143">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="349bb-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="349bb-144">errorCode</span></span>|[<span data-ttu-id="349bb-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="349bb-145">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="349bb-146">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="349bb-146">Error code if any occured.</span></span> <span data-ttu-id="349bb-147">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="349bb-147">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="349bb-148">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="349bb-148">guidedDeploymentTags</span></span>|<span data-ttu-id="349bb-149">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="349bb-149">String collection</span></span>|<span data-ttu-id="349bb-150">Теги в руководстве по развертыванию</span><span class="sxs-lookup"><span data-stu-id="349bb-150">Tags of the guided deployment</span></span>|

## <a name="relationships"></a><span data-ttu-id="349bb-151">Связи</span><span class="sxs-lookup"><span data-stu-id="349bb-151">Relationships</span></span>
<span data-ttu-id="349bb-152">Нет</span><span class="sxs-lookup"><span data-stu-id="349bb-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="349bb-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="349bb-153">JSON Representation</span></span>
<span data-ttu-id="349bb-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="349bb-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```



