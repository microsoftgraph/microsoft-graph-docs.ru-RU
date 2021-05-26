---
title: тип ресурса deviceManagementConfigurationSettingValueTemplateReference
description: Настройка справочной информации шаблона значений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa4ecc07044d90bfc869467de8e8249f7581e228
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667052"
---
# <a name="devicemanagementconfigurationsettingvaluetemplatereference-resource-type"></a><span data-ttu-id="bbb32-103">тип ресурса deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="bbb32-103">deviceManagementConfigurationSettingValueTemplateReference resource type</span></span>

<span data-ttu-id="bbb32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbb32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbb32-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbb32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbb32-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbb32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbb32-107">Настройка справочной информации шаблона значений</span><span class="sxs-lookup"><span data-stu-id="bbb32-107">Setting value template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="bbb32-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbb32-108">Properties</span></span>
|<span data-ttu-id="bbb32-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbb32-109">Property</span></span>|<span data-ttu-id="bbb32-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bbb32-110">Type</span></span>|<span data-ttu-id="bbb32-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bbb32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbb32-112">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="bbb32-112">settingValueTemplateId</span></span>|<span data-ttu-id="bbb32-113">Строка</span><span class="sxs-lookup"><span data-stu-id="bbb32-113">String</span></span>|<span data-ttu-id="bbb32-114">Настройка id шаблона значений</span><span class="sxs-lookup"><span data-stu-id="bbb32-114">Setting value template id</span></span>|
|<span data-ttu-id="bbb32-115">useTemplateDefault</span><span class="sxs-lookup"><span data-stu-id="bbb32-115">useTemplateDefault</span></span>|<span data-ttu-id="bbb32-116">Логический</span><span class="sxs-lookup"><span data-stu-id="bbb32-116">Boolean</span></span>|<span data-ttu-id="bbb32-117">Указывает, следует ли обновлять значение параметра политики, чтобы соответствовать значению параметра шаблона по умолчанию</span><span class="sxs-lookup"><span data-stu-id="bbb32-117">Indicates whether to update policy setting value to match template setting default value</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbb32-118">Связи</span><span class="sxs-lookup"><span data-stu-id="bbb32-118">Relationships</span></span>
<span data-ttu-id="bbb32-119">Нет</span><span class="sxs-lookup"><span data-stu-id="bbb32-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbb32-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbb32-120">JSON Representation</span></span>
<span data-ttu-id="bbb32-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbb32-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
  "settingValueTemplateId": "String",
  "useTemplateDefault": true
}
```




