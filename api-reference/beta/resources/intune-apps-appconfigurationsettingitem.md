---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
ms.openlocfilehash: c0e340374b9dfc43b80fa310923785c0475a9532
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078828"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="d7533-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="d7533-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="d7533-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7533-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7533-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7533-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7533-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d7533-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7533-107">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="d7533-107">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="d7533-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7533-108">Properties</span></span>
|<span data-ttu-id="d7533-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7533-109">Property</span></span>|<span data-ttu-id="d7533-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d7533-110">Type</span></span>|<span data-ttu-id="d7533-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7533-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7533-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="d7533-112">appConfigKey</span></span>|<span data-ttu-id="d7533-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d7533-113">String</span></span>|<span data-ttu-id="d7533-114">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="d7533-114">app configuration key.</span></span>|
|<span data-ttu-id="d7533-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d7533-115">appConfigKeyType</span></span>|[<span data-ttu-id="d7533-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d7533-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="d7533-117">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="d7533-117">app configuration key type.</span></span> <span data-ttu-id="d7533-118">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="d7533-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="d7533-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="d7533-119">appConfigKeyValue</span></span>|<span data-ttu-id="d7533-120">Строка</span><span class="sxs-lookup"><span data-stu-id="d7533-120">String</span></span>|<span data-ttu-id="d7533-121">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="d7533-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7533-122">Связи</span><span class="sxs-lookup"><span data-stu-id="d7533-122">Relationships</span></span>
<span data-ttu-id="d7533-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d7533-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d7533-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7533-124">JSON Representation</span></span>
<span data-ttu-id="d7533-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7533-125">Here is a JSON representation of the resource.</span></span>
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





