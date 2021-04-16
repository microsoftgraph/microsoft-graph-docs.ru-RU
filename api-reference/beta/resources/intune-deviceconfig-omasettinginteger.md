---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19db5504d276c748d720803ba201c555752e2f33
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867394"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="90e48-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="90e48-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="90e48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90e48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90e48-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90e48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90e48-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90e48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90e48-107">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="90e48-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="90e48-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="90e48-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="90e48-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="90e48-109">Properties</span></span>
|<span data-ttu-id="90e48-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="90e48-110">Property</span></span>|<span data-ttu-id="90e48-111">Тип</span><span class="sxs-lookup"><span data-stu-id="90e48-111">Type</span></span>|<span data-ttu-id="90e48-112">Описание</span><span class="sxs-lookup"><span data-stu-id="90e48-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90e48-113">displayName</span><span class="sxs-lookup"><span data-stu-id="90e48-113">displayName</span></span>|<span data-ttu-id="90e48-114">String</span><span class="sxs-lookup"><span data-stu-id="90e48-114">String</span></span>|<span data-ttu-id="90e48-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="90e48-115">Display Name.</span></span> <span data-ttu-id="90e48-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="90e48-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="90e48-117">description</span><span class="sxs-lookup"><span data-stu-id="90e48-117">description</span></span>|<span data-ttu-id="90e48-118">String</span><span class="sxs-lookup"><span data-stu-id="90e48-118">String</span></span>|<span data-ttu-id="90e48-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="90e48-119">Description.</span></span> <span data-ttu-id="90e48-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="90e48-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="90e48-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="90e48-121">omaUri</span></span>|<span data-ttu-id="90e48-122">String</span><span class="sxs-lookup"><span data-stu-id="90e48-122">String</span></span>|<span data-ttu-id="90e48-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="90e48-123">OMA.</span></span> <span data-ttu-id="90e48-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="90e48-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="90e48-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="90e48-125">secretReferenceValueId</span></span>|<span data-ttu-id="90e48-126">String</span><span class="sxs-lookup"><span data-stu-id="90e48-126">String</span></span>|<span data-ttu-id="90e48-127">ReferenceId для поисков секрета для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="90e48-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="90e48-128">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="90e48-128">This property is read-only.</span></span> <span data-ttu-id="90e48-129">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="90e48-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="90e48-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="90e48-130">isEncrypted</span></span>|<span data-ttu-id="90e48-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="90e48-131">Boolean</span></span>|<span data-ttu-id="90e48-132">Указывает, зашифровано ли поле значений.</span><span class="sxs-lookup"><span data-stu-id="90e48-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="90e48-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="90e48-133">This property is read-only.</span></span> <span data-ttu-id="90e48-134">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="90e48-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="90e48-135">value</span><span class="sxs-lookup"><span data-stu-id="90e48-135">value</span></span>|<span data-ttu-id="90e48-136">Int32</span><span class="sxs-lookup"><span data-stu-id="90e48-136">Int32</span></span>|<span data-ttu-id="90e48-137">Значение.</span><span class="sxs-lookup"><span data-stu-id="90e48-137">Value.</span></span>|
|<span data-ttu-id="90e48-138">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="90e48-138">isReadOnly</span></span>|<span data-ttu-id="90e48-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="90e48-139">Boolean</span></span>|<span data-ttu-id="90e48-140">Установив true, CSP (поставщик служб конфигурации), указанный в OMA-URI, выполнит get, а не set</span><span class="sxs-lookup"><span data-stu-id="90e48-140">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="90e48-141">Связи</span><span class="sxs-lookup"><span data-stu-id="90e48-141">Relationships</span></span>
<span data-ttu-id="90e48-142">Нет</span><span class="sxs-lookup"><span data-stu-id="90e48-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90e48-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90e48-143">JSON Representation</span></span>
<span data-ttu-id="90e48-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90e48-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": 1024,
  "isReadOnly": true
}
```




