---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9710c40e92e3cb1d5416b54b589de5305ed44c8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368473"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="d7ff6-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="d7ff6-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="d7ff6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7ff6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7ff6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7ff6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7ff6-106">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="d7ff6-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="d7ff6-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d7ff6-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7ff6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7ff6-108">Properties</span></span>
|<span data-ttu-id="d7ff6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7ff6-109">Property</span></span>|<span data-ttu-id="d7ff6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d7ff6-110">Type</span></span>|<span data-ttu-id="d7ff6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7ff6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7ff6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d7ff6-112">displayName</span></span>|<span data-ttu-id="d7ff6-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d7ff6-113">String</span></span>|<span data-ttu-id="d7ff6-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d7ff6-114">Display Name.</span></span> <span data-ttu-id="d7ff6-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d7ff6-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d7ff6-116">description</span><span class="sxs-lookup"><span data-stu-id="d7ff6-116">description</span></span>|<span data-ttu-id="d7ff6-117">String</span><span class="sxs-lookup"><span data-stu-id="d7ff6-117">String</span></span>|<span data-ttu-id="d7ff6-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="d7ff6-118">Description.</span></span> <span data-ttu-id="d7ff6-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d7ff6-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d7ff6-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="d7ff6-120">omaUri</span></span>|<span data-ttu-id="d7ff6-121">String</span><span class="sxs-lookup"><span data-stu-id="d7ff6-121">String</span></span>|<span data-ttu-id="d7ff6-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="d7ff6-122">OMA.</span></span> <span data-ttu-id="d7ff6-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d7ff6-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d7ff6-124">value</span><span class="sxs-lookup"><span data-stu-id="d7ff6-124">value</span></span>|<span data-ttu-id="d7ff6-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d7ff6-125">Int32</span></span>|<span data-ttu-id="d7ff6-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="d7ff6-126">Value.</span></span>|
|<span data-ttu-id="d7ff6-127">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="d7ff6-127">isReadOnly</span></span>|<span data-ttu-id="d7ff6-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7ff6-128">Boolean</span></span>|<span data-ttu-id="d7ff6-129">Если задано значение true, CSP (поставщик услуг по настройке), указанный в OMA-URI, будет выполнять Get, а не Set</span><span class="sxs-lookup"><span data-stu-id="d7ff6-129">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7ff6-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="d7ff6-130">Relationships</span></span>
<span data-ttu-id="d7ff6-131">Нет</span><span class="sxs-lookup"><span data-stu-id="d7ff6-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7ff6-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7ff6-132">JSON Representation</span></span>
<span data-ttu-id="d7ff6-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7ff6-133">Here is a JSON representation of the resource.</span></span>
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
  "value": 1024,
  "isReadOnly": true
}
```



