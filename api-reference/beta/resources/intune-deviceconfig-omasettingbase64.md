---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67fcf5574b3cb4481286ecc7b4448018d64e0f44
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472029"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="92f48-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="92f48-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="92f48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92f48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92f48-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92f48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92f48-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92f48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92f48-107">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="92f48-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="92f48-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="92f48-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92f48-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="92f48-109">Properties</span></span>
|<span data-ttu-id="92f48-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="92f48-110">Property</span></span>|<span data-ttu-id="92f48-111">Тип</span><span class="sxs-lookup"><span data-stu-id="92f48-111">Type</span></span>|<span data-ttu-id="92f48-112">Описание</span><span class="sxs-lookup"><span data-stu-id="92f48-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92f48-113">displayName</span><span class="sxs-lookup"><span data-stu-id="92f48-113">displayName</span></span>|<span data-ttu-id="92f48-114">String</span><span class="sxs-lookup"><span data-stu-id="92f48-114">String</span></span>|<span data-ttu-id="92f48-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="92f48-115">Display Name.</span></span> <span data-ttu-id="92f48-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="92f48-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="92f48-117">description</span><span class="sxs-lookup"><span data-stu-id="92f48-117">description</span></span>|<span data-ttu-id="92f48-118">String</span><span class="sxs-lookup"><span data-stu-id="92f48-118">String</span></span>|<span data-ttu-id="92f48-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="92f48-119">Description.</span></span> <span data-ttu-id="92f48-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="92f48-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="92f48-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="92f48-121">omaUri</span></span>|<span data-ttu-id="92f48-122">String</span><span class="sxs-lookup"><span data-stu-id="92f48-122">String</span></span>|<span data-ttu-id="92f48-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="92f48-123">OMA.</span></span> <span data-ttu-id="92f48-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="92f48-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="92f48-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="92f48-125">isEncrypted</span></span>|<span data-ttu-id="92f48-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="92f48-126">Boolean</span></span>|<span data-ttu-id="92f48-127">Указывает, зашифровано ли поле значений.</span><span class="sxs-lookup"><span data-stu-id="92f48-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="92f48-128">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="92f48-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="92f48-129">fileName</span><span class="sxs-lookup"><span data-stu-id="92f48-129">fileName</span></span>|<span data-ttu-id="92f48-130">String</span><span class="sxs-lookup"><span data-stu-id="92f48-130">String</span></span>|<span data-ttu-id="92f48-131">Имя файла, связанное с свойством Value (\*.cer \| \*.crt \| \*.p7b \| \*.bin).</span><span class="sxs-lookup"><span data-stu-id="92f48-131">File name associated with the Value property (\*.cer \| \*.crt \| \*.p7b \| \*.bin).</span></span>|
|<span data-ttu-id="92f48-132">value</span><span class="sxs-lookup"><span data-stu-id="92f48-132">value</span></span>|<span data-ttu-id="92f48-133">String</span><span class="sxs-lookup"><span data-stu-id="92f48-133">String</span></span>|<span data-ttu-id="92f48-134">Значение</span><span class="sxs-lookup"><span data-stu-id="92f48-134">Value.</span></span> <span data-ttu-id="92f48-135">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="92f48-135">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="92f48-136">Связи</span><span class="sxs-lookup"><span data-stu-id="92f48-136">Relationships</span></span>
<span data-ttu-id="92f48-137">Нет</span><span class="sxs-lookup"><span data-stu-id="92f48-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92f48-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92f48-138">JSON Representation</span></span>
<span data-ttu-id="92f48-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92f48-139">Here is a JSON representation of the resource.</span></span>
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
  "isEncrypted": true,
  "fileName": "String",
  "value": "String"
}
```




