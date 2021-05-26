---
title: тип ресурса deviceManagementConfigurationSettingInstanceTemplateReference
description: Настройка справочной информации шаблона экземпляра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d537791337f13ba9fcf3bd19ef77b1c0aec58463
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667058"
---
# <a name="devicemanagementconfigurationsettinginstancetemplatereference-resource-type"></a><span data-ttu-id="56539-103">тип ресурса deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="56539-103">deviceManagementConfigurationSettingInstanceTemplateReference resource type</span></span>

<span data-ttu-id="56539-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56539-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56539-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56539-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56539-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56539-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56539-107">Настройка справочной информации шаблона экземпляра</span><span class="sxs-lookup"><span data-stu-id="56539-107">Setting instance template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="56539-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="56539-108">Properties</span></span>
|<span data-ttu-id="56539-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="56539-109">Property</span></span>|<span data-ttu-id="56539-110">Тип</span><span class="sxs-lookup"><span data-stu-id="56539-110">Type</span></span>|<span data-ttu-id="56539-111">Описание</span><span class="sxs-lookup"><span data-stu-id="56539-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56539-112">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="56539-112">settingInstanceTemplateId</span></span>|<span data-ttu-id="56539-113">Строка</span><span class="sxs-lookup"><span data-stu-id="56539-113">String</span></span>|<span data-ttu-id="56539-114">Настройка кода шаблона экземпляра</span><span class="sxs-lookup"><span data-stu-id="56539-114">Setting instance template id</span></span>|

## <a name="relationships"></a><span data-ttu-id="56539-115">Связи</span><span class="sxs-lookup"><span data-stu-id="56539-115">Relationships</span></span>
<span data-ttu-id="56539-116">Нет</span><span class="sxs-lookup"><span data-stu-id="56539-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56539-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56539-117">JSON Representation</span></span>
<span data-ttu-id="56539-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56539-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
  "settingInstanceTemplateId": "String"
}
```




