---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7f5492c9b54c9414db6a8332e218a1d7f0a50b1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403765"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="46e0d-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="46e0d-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="46e0d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46e0d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46e0d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46e0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46e0d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46e0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46e0d-107">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="46e0d-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="46e0d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="46e0d-108">Properties</span></span>
|<span data-ttu-id="46e0d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="46e0d-109">Property</span></span>|<span data-ttu-id="46e0d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="46e0d-110">Type</span></span>|<span data-ttu-id="46e0d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="46e0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46e0d-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="46e0d-112">appConfigKey</span></span>|<span data-ttu-id="46e0d-113">Строка</span><span class="sxs-lookup"><span data-stu-id="46e0d-113">String</span></span>|<span data-ttu-id="46e0d-114">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="46e0d-114">app configuration key.</span></span>|
|<span data-ttu-id="46e0d-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="46e0d-115">appConfigKeyType</span></span>|[<span data-ttu-id="46e0d-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="46e0d-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="46e0d-117">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="46e0d-117">app configuration key type.</span></span> <span data-ttu-id="46e0d-118">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="46e0d-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="46e0d-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="46e0d-119">appConfigKeyValue</span></span>|<span data-ttu-id="46e0d-120">Строка</span><span class="sxs-lookup"><span data-stu-id="46e0d-120">String</span></span>|<span data-ttu-id="46e0d-121">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="46e0d-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46e0d-122">Связи</span><span class="sxs-lookup"><span data-stu-id="46e0d-122">Relationships</span></span>
<span data-ttu-id="46e0d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="46e0d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46e0d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46e0d-124">JSON Representation</span></span>
<span data-ttu-id="46e0d-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46e0d-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```




