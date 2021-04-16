---
title: тип ресурса deviceManagementConfigurationSettingInstanceTemplate
description: Настройка шаблона экземпляра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76d8c9b985a3ca30f0d2a0a4144128d0e7a1baff
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868986"
---
# <a name="devicemanagementconfigurationsettinginstancetemplate-resource-type"></a><span data-ttu-id="49639-103">тип ресурса deviceManagementConfigurationSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="49639-103">deviceManagementConfigurationSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="49639-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49639-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49639-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49639-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49639-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49639-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49639-107">Настройка шаблона экземпляра</span><span class="sxs-lookup"><span data-stu-id="49639-107">Setting Instance Template</span></span>

## <a name="properties"></a><span data-ttu-id="49639-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="49639-108">Properties</span></span>
|<span data-ttu-id="49639-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="49639-109">Property</span></span>|<span data-ttu-id="49639-110">Тип</span><span class="sxs-lookup"><span data-stu-id="49639-110">Type</span></span>|<span data-ttu-id="49639-111">Описание</span><span class="sxs-lookup"><span data-stu-id="49639-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49639-112">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="49639-112">settingInstanceTemplateId</span></span>|<span data-ttu-id="49639-113">String</span><span class="sxs-lookup"><span data-stu-id="49639-113">String</span></span>|<span data-ttu-id="49639-114">Настройка кода шаблона экземпляра</span><span class="sxs-lookup"><span data-stu-id="49639-114">Setting Instance Template Id</span></span>|
|<span data-ttu-id="49639-115">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="49639-115">settingDefinitionId</span></span>|<span data-ttu-id="49639-116">String</span><span class="sxs-lookup"><span data-stu-id="49639-116">String</span></span>|<span data-ttu-id="49639-117">Настройка Id определения</span><span class="sxs-lookup"><span data-stu-id="49639-117">Setting Definition Id</span></span>|
|<span data-ttu-id="49639-118">isRequired</span><span class="sxs-lookup"><span data-stu-id="49639-118">isRequired</span></span>|<span data-ttu-id="49639-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="49639-119">Boolean</span></span>|<span data-ttu-id="49639-120">Указывает, должна ли политика указать этот параметр.</span><span class="sxs-lookup"><span data-stu-id="49639-120">Indicates if a policy must specify this setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49639-121">Связи</span><span class="sxs-lookup"><span data-stu-id="49639-121">Relationships</span></span>
<span data-ttu-id="49639-122">Нет</span><span class="sxs-lookup"><span data-stu-id="49639-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49639-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49639-123">JSON Representation</span></span>
<span data-ttu-id="49639-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49639-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true
}
```




