---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30ed623b5fc59b9a96c0e37e8b2b1fcfc77e7b13
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867429"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="31a54-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="31a54-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="31a54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31a54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31a54-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31a54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31a54-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31a54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31a54-107">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="31a54-107">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="31a54-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="31a54-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="31a54-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="31a54-109">Properties</span></span>
|<span data-ttu-id="31a54-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="31a54-110">Property</span></span>|<span data-ttu-id="31a54-111">Тип</span><span class="sxs-lookup"><span data-stu-id="31a54-111">Type</span></span>|<span data-ttu-id="31a54-112">Описание</span><span class="sxs-lookup"><span data-stu-id="31a54-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31a54-113">displayName</span><span class="sxs-lookup"><span data-stu-id="31a54-113">displayName</span></span>|<span data-ttu-id="31a54-114">String</span><span class="sxs-lookup"><span data-stu-id="31a54-114">String</span></span>|<span data-ttu-id="31a54-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="31a54-115">Display Name.</span></span> <span data-ttu-id="31a54-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="31a54-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="31a54-117">description</span><span class="sxs-lookup"><span data-stu-id="31a54-117">description</span></span>|<span data-ttu-id="31a54-118">String</span><span class="sxs-lookup"><span data-stu-id="31a54-118">String</span></span>|<span data-ttu-id="31a54-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="31a54-119">Description.</span></span> <span data-ttu-id="31a54-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="31a54-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="31a54-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="31a54-121">omaUri</span></span>|<span data-ttu-id="31a54-122">String</span><span class="sxs-lookup"><span data-stu-id="31a54-122">String</span></span>|<span data-ttu-id="31a54-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="31a54-123">OMA.</span></span> <span data-ttu-id="31a54-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="31a54-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="31a54-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="31a54-125">secretReferenceValueId</span></span>|<span data-ttu-id="31a54-126">String</span><span class="sxs-lookup"><span data-stu-id="31a54-126">String</span></span>|<span data-ttu-id="31a54-127">ReferenceId для поисков секрета для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="31a54-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="31a54-128">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31a54-128">This property is read-only.</span></span> <span data-ttu-id="31a54-129">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="31a54-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="31a54-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="31a54-130">isEncrypted</span></span>|<span data-ttu-id="31a54-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="31a54-131">Boolean</span></span>|<span data-ttu-id="31a54-132">Указывает, зашифровано ли поле значений.</span><span class="sxs-lookup"><span data-stu-id="31a54-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="31a54-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31a54-133">This property is read-only.</span></span> <span data-ttu-id="31a54-134">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="31a54-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="31a54-135">value</span><span class="sxs-lookup"><span data-stu-id="31a54-135">value</span></span>|<span data-ttu-id="31a54-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31a54-136">DateTimeOffset</span></span>|<span data-ttu-id="31a54-137">Значение.</span><span class="sxs-lookup"><span data-stu-id="31a54-137">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31a54-138">Связи</span><span class="sxs-lookup"><span data-stu-id="31a54-138">Relationships</span></span>
<span data-ttu-id="31a54-139">Нет</span><span class="sxs-lookup"><span data-stu-id="31a54-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31a54-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31a54-140">JSON Representation</span></span>
<span data-ttu-id="31a54-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31a54-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": "String (timestamp)"
}
```




