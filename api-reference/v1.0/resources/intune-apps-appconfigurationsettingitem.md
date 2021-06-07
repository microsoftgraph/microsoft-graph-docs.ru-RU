---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af738e6c5f558b7460c8cbd7c5e02abae3dbb922
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756087"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="85d53-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="85d53-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="85d53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85d53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85d53-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85d53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85d53-106">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="85d53-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="85d53-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="85d53-107">Properties</span></span>
|<span data-ttu-id="85d53-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="85d53-108">Property</span></span>|<span data-ttu-id="85d53-109">Тип</span><span class="sxs-lookup"><span data-stu-id="85d53-109">Type</span></span>|<span data-ttu-id="85d53-110">Описание</span><span class="sxs-lookup"><span data-stu-id="85d53-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85d53-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="85d53-111">appConfigKey</span></span>|<span data-ttu-id="85d53-112">Строка</span><span class="sxs-lookup"><span data-stu-id="85d53-112">String</span></span>|<span data-ttu-id="85d53-113">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="85d53-113">app configuration key.</span></span>|
|<span data-ttu-id="85d53-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="85d53-114">appConfigKeyType</span></span>|[<span data-ttu-id="85d53-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="85d53-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="85d53-116">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="85d53-116">app configuration key type.</span></span> <span data-ttu-id="85d53-117">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="85d53-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="85d53-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="85d53-118">appConfigKeyValue</span></span>|<span data-ttu-id="85d53-119">Строка</span><span class="sxs-lookup"><span data-stu-id="85d53-119">String</span></span>|<span data-ttu-id="85d53-120">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="85d53-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85d53-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="85d53-121">Relationships</span></span>
<span data-ttu-id="85d53-122">Нет</span><span class="sxs-lookup"><span data-stu-id="85d53-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85d53-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85d53-123">JSON Representation</span></span>
<span data-ttu-id="85d53-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85d53-124">Here is a JSON representation of the resource.</span></span>
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




