---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11ef3a964d166301c04c49730ac084b68e700b7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503592"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="7a7ad-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="7a7ad-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="7a7ad-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a7ad-105">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="7a7ad-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a7ad-106">Properties</span></span>
|<span data-ttu-id="7a7ad-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a7ad-107">Property</span></span>|<span data-ttu-id="7a7ad-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7a7ad-108">Type</span></span>|<span data-ttu-id="7a7ad-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7a7ad-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a7ad-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="7a7ad-110">appConfigKey</span></span>|<span data-ttu-id="7a7ad-111">String</span><span class="sxs-lookup"><span data-stu-id="7a7ad-111">String</span></span>|<span data-ttu-id="7a7ad-112">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-112">app configuration key.</span></span>|
|<span data-ttu-id="7a7ad-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="7a7ad-113">appConfigKeyType</span></span>|[<span data-ttu-id="7a7ad-114">Мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="7a7ad-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="7a7ad-115">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-115">app configuration key type.</span></span> <span data-ttu-id="7a7ad-116">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="7a7ad-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="7a7ad-117">appConfigKeyValue</span></span>|<span data-ttu-id="7a7ad-118">Строка</span><span class="sxs-lookup"><span data-stu-id="7a7ad-118">String</span></span>|<span data-ttu-id="7a7ad-119">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a7ad-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="7a7ad-120">Relationships</span></span>
<span data-ttu-id="7a7ad-121">Нет</span><span class="sxs-lookup"><span data-stu-id="7a7ad-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a7ad-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a7ad-122">JSON Representation</span></span>
<span data-ttu-id="7a7ad-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-123">Here is a JSON representation of the resource.</span></span>
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



