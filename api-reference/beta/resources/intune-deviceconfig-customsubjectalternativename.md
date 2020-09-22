---
title: Тип ресурса Кустомсубжекталтернативенаме
description: Определение альтернативного имени настраиваемой темы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06fcded3c2e59fd13c90b5605dcc04df354a2e8a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061989"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="015cf-103">Тип ресурса Кустомсубжекталтернативенаме</span><span class="sxs-lookup"><span data-stu-id="015cf-103">customSubjectAlternativeName resource type</span></span>

<span data-ttu-id="015cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="015cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="015cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="015cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="015cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="015cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="015cf-107">Определение альтернативного имени настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="015cf-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="015cf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="015cf-108">Properties</span></span>
|<span data-ttu-id="015cf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="015cf-109">Property</span></span>|<span data-ttu-id="015cf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="015cf-110">Type</span></span>|<span data-ttu-id="015cf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="015cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="015cf-112">сантипе</span><span class="sxs-lookup"><span data-stu-id="015cf-112">sanType</span></span>|[<span data-ttu-id="015cf-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="015cf-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="015cf-114">Настраиваемый тип SAN.</span><span class="sxs-lookup"><span data-stu-id="015cf-114">Custom SAN Type.</span></span> <span data-ttu-id="015cf-115">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="015cf-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="015cf-116">name</span><span class="sxs-lookup"><span data-stu-id="015cf-116">name</span></span>|<span data-ttu-id="015cf-117">String</span><span class="sxs-lookup"><span data-stu-id="015cf-117">String</span></span>|<span data-ttu-id="015cf-118">Настраиваемое имя сети хранения данных</span><span class="sxs-lookup"><span data-stu-id="015cf-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="015cf-119">Связи</span><span class="sxs-lookup"><span data-stu-id="015cf-119">Relationships</span></span>
<span data-ttu-id="015cf-120">Нет</span><span class="sxs-lookup"><span data-stu-id="015cf-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="015cf-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="015cf-121">JSON Representation</span></span>
<span data-ttu-id="015cf-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="015cf-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```






