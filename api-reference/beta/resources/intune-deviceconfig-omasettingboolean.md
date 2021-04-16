---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e1118001a06ff19439d5d0b1a3970b358235f4d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867443"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="165e2-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="165e2-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="165e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="165e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="165e2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="165e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="165e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="165e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="165e2-107">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="165e2-107">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="165e2-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="165e2-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="165e2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="165e2-109">Properties</span></span>
|<span data-ttu-id="165e2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="165e2-110">Property</span></span>|<span data-ttu-id="165e2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="165e2-111">Type</span></span>|<span data-ttu-id="165e2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="165e2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="165e2-113">displayName</span><span class="sxs-lookup"><span data-stu-id="165e2-113">displayName</span></span>|<span data-ttu-id="165e2-114">String</span><span class="sxs-lookup"><span data-stu-id="165e2-114">String</span></span>|<span data-ttu-id="165e2-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="165e2-115">Display Name.</span></span> <span data-ttu-id="165e2-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="165e2-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="165e2-117">description</span><span class="sxs-lookup"><span data-stu-id="165e2-117">description</span></span>|<span data-ttu-id="165e2-118">String</span><span class="sxs-lookup"><span data-stu-id="165e2-118">String</span></span>|<span data-ttu-id="165e2-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="165e2-119">Description.</span></span> <span data-ttu-id="165e2-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="165e2-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="165e2-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="165e2-121">omaUri</span></span>|<span data-ttu-id="165e2-122">String</span><span class="sxs-lookup"><span data-stu-id="165e2-122">String</span></span>|<span data-ttu-id="165e2-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="165e2-123">OMA.</span></span> <span data-ttu-id="165e2-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="165e2-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="165e2-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="165e2-125">secretReferenceValueId</span></span>|<span data-ttu-id="165e2-126">String</span><span class="sxs-lookup"><span data-stu-id="165e2-126">String</span></span>|<span data-ttu-id="165e2-127">ReferenceId для поисков секрета для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="165e2-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="165e2-128">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="165e2-128">This property is read-only.</span></span> <span data-ttu-id="165e2-129">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="165e2-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="165e2-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="165e2-130">isEncrypted</span></span>|<span data-ttu-id="165e2-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="165e2-131">Boolean</span></span>|<span data-ttu-id="165e2-132">Указывает, зашифровано ли поле значений.</span><span class="sxs-lookup"><span data-stu-id="165e2-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="165e2-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="165e2-133">This property is read-only.</span></span> <span data-ttu-id="165e2-134">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="165e2-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="165e2-135">value</span><span class="sxs-lookup"><span data-stu-id="165e2-135">value</span></span>|<span data-ttu-id="165e2-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="165e2-136">Boolean</span></span>|<span data-ttu-id="165e2-137">Значение</span><span class="sxs-lookup"><span data-stu-id="165e2-137">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="165e2-138">Связи</span><span class="sxs-lookup"><span data-stu-id="165e2-138">Relationships</span></span>
<span data-ttu-id="165e2-139">Нет</span><span class="sxs-lookup"><span data-stu-id="165e2-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="165e2-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="165e2-140">JSON Representation</span></span>
<span data-ttu-id="165e2-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="165e2-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": true
}
```




