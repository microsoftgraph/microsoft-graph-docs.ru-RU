---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b899a076a291061649adab4724a9108d982886f5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867373"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="76b71-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="76b71-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="76b71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76b71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76b71-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76b71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76b71-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76b71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76b71-107">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="76b71-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="76b71-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="76b71-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="76b71-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="76b71-109">Properties</span></span>
|<span data-ttu-id="76b71-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="76b71-110">Property</span></span>|<span data-ttu-id="76b71-111">Тип</span><span class="sxs-lookup"><span data-stu-id="76b71-111">Type</span></span>|<span data-ttu-id="76b71-112">Описание</span><span class="sxs-lookup"><span data-stu-id="76b71-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76b71-113">displayName</span><span class="sxs-lookup"><span data-stu-id="76b71-113">displayName</span></span>|<span data-ttu-id="76b71-114">String</span><span class="sxs-lookup"><span data-stu-id="76b71-114">String</span></span>|<span data-ttu-id="76b71-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="76b71-115">Display Name.</span></span> <span data-ttu-id="76b71-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="76b71-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="76b71-117">description</span><span class="sxs-lookup"><span data-stu-id="76b71-117">description</span></span>|<span data-ttu-id="76b71-118">String</span><span class="sxs-lookup"><span data-stu-id="76b71-118">String</span></span>|<span data-ttu-id="76b71-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="76b71-119">Description.</span></span> <span data-ttu-id="76b71-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="76b71-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="76b71-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="76b71-121">omaUri</span></span>|<span data-ttu-id="76b71-122">String</span><span class="sxs-lookup"><span data-stu-id="76b71-122">String</span></span>|<span data-ttu-id="76b71-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="76b71-123">OMA.</span></span> <span data-ttu-id="76b71-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="76b71-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="76b71-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="76b71-125">secretReferenceValueId</span></span>|<span data-ttu-id="76b71-126">String</span><span class="sxs-lookup"><span data-stu-id="76b71-126">String</span></span>|<span data-ttu-id="76b71-127">ReferenceId для поисков секрета для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="76b71-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="76b71-128">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76b71-128">This property is read-only.</span></span> <span data-ttu-id="76b71-129">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="76b71-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="76b71-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="76b71-130">isEncrypted</span></span>|<span data-ttu-id="76b71-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="76b71-131">Boolean</span></span>|<span data-ttu-id="76b71-132">Указывает, зашифровано ли поле значений.</span><span class="sxs-lookup"><span data-stu-id="76b71-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="76b71-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76b71-133">This property is read-only.</span></span> <span data-ttu-id="76b71-134">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="76b71-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="76b71-135">fileName</span><span class="sxs-lookup"><span data-stu-id="76b71-135">fileName</span></span>|<span data-ttu-id="76b71-136">String</span><span class="sxs-lookup"><span data-stu-id="76b71-136">String</span></span>|<span data-ttu-id="76b71-137">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="76b71-137">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="76b71-138">value</span><span class="sxs-lookup"><span data-stu-id="76b71-138">value</span></span>|<span data-ttu-id="76b71-139">Двоичный</span><span class="sxs-lookup"><span data-stu-id="76b71-139">Binary</span></span>|<span data-ttu-id="76b71-140">Значение</span><span class="sxs-lookup"><span data-stu-id="76b71-140">Value.</span></span> <span data-ttu-id="76b71-141">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="76b71-141">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="76b71-142">Связи</span><span class="sxs-lookup"><span data-stu-id="76b71-142">Relationships</span></span>
<span data-ttu-id="76b71-143">Нет</span><span class="sxs-lookup"><span data-stu-id="76b71-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76b71-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76b71-144">JSON Representation</span></span>
<span data-ttu-id="76b71-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76b71-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "fileName": "String",
  "value": "binary"
}
```




