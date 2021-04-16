---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8729dd6251f9dbaf062fbfee3d024de265565020
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867457"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="aeaa3-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="aeaa3-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="aeaa3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aeaa3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aeaa3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aeaa3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aeaa3-107">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="aeaa3-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aeaa3-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aeaa3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="aeaa3-109">Properties</span></span>
|<span data-ttu-id="aeaa3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="aeaa3-110">Property</span></span>|<span data-ttu-id="aeaa3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="aeaa3-111">Type</span></span>|<span data-ttu-id="aeaa3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="aeaa3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeaa3-113">displayName</span><span class="sxs-lookup"><span data-stu-id="aeaa3-113">displayName</span></span>|<span data-ttu-id="aeaa3-114">String</span><span class="sxs-lookup"><span data-stu-id="aeaa3-114">String</span></span>|<span data-ttu-id="aeaa3-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-115">Display Name.</span></span> <span data-ttu-id="aeaa3-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aeaa3-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="aeaa3-117">description</span><span class="sxs-lookup"><span data-stu-id="aeaa3-117">description</span></span>|<span data-ttu-id="aeaa3-118">String</span><span class="sxs-lookup"><span data-stu-id="aeaa3-118">String</span></span>|<span data-ttu-id="aeaa3-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-119">Description.</span></span> <span data-ttu-id="aeaa3-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aeaa3-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="aeaa3-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="aeaa3-121">omaUri</span></span>|<span data-ttu-id="aeaa3-122">String</span><span class="sxs-lookup"><span data-stu-id="aeaa3-122">String</span></span>|<span data-ttu-id="aeaa3-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-123">OMA.</span></span> <span data-ttu-id="aeaa3-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aeaa3-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="aeaa3-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="aeaa3-125">secretReferenceValueId</span></span>|<span data-ttu-id="aeaa3-126">String</span><span class="sxs-lookup"><span data-stu-id="aeaa3-126">String</span></span>|<span data-ttu-id="aeaa3-127">ReferenceId для поисков секрета для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="aeaa3-128">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-128">This property is read-only.</span></span> <span data-ttu-id="aeaa3-129">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aeaa3-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="aeaa3-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="aeaa3-130">isEncrypted</span></span>|<span data-ttu-id="aeaa3-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeaa3-131">Boolean</span></span>|<span data-ttu-id="aeaa3-132">Указывает, зашифровано ли поле значений.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="aeaa3-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-133">This property is read-only.</span></span> <span data-ttu-id="aeaa3-134">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aeaa3-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="aeaa3-135">fileName</span><span class="sxs-lookup"><span data-stu-id="aeaa3-135">fileName</span></span>|<span data-ttu-id="aeaa3-136">String</span><span class="sxs-lookup"><span data-stu-id="aeaa3-136">String</span></span>|<span data-ttu-id="aeaa3-137">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="aeaa3-137">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="aeaa3-138">\*.crt</span><span class="sxs-lookup"><span data-stu-id="aeaa3-138">\*.crt</span></span> | <span data-ttu-id="aeaa3-139">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="aeaa3-139">\*.p7b</span></span> | <span data-ttu-id="aeaa3-140">\*.bin).</span><span class="sxs-lookup"><span data-stu-id="aeaa3-140">\*.bin).</span></span>|
|<span data-ttu-id="aeaa3-141">value</span><span class="sxs-lookup"><span data-stu-id="aeaa3-141">value</span></span>|<span data-ttu-id="aeaa3-142">String</span><span class="sxs-lookup"><span data-stu-id="aeaa3-142">String</span></span>|<span data-ttu-id="aeaa3-143">Значение</span><span class="sxs-lookup"><span data-stu-id="aeaa3-143">Value.</span></span> <span data-ttu-id="aeaa3-144">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="aeaa3-144">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="aeaa3-145">Связи</span><span class="sxs-lookup"><span data-stu-id="aeaa3-145">Relationships</span></span>
<span data-ttu-id="aeaa3-146">Нет</span><span class="sxs-lookup"><span data-stu-id="aeaa3-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aeaa3-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aeaa3-147">JSON Representation</span></span>
<span data-ttu-id="aeaa3-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aeaa3-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "fileName": "String",
  "value": "String"
}
```




