---
title: Тип ресурса Кустомсубжекталтернативенаме
description: Определение альтернативного имени настраиваемой темы
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03507d4e912af011db011283a95887590ab79801
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549374"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="8c68b-103">Тип ресурса Кустомсубжекталтернативенаме</span><span class="sxs-lookup"><span data-stu-id="8c68b-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="8c68b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c68b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c68b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c68b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c68b-106">Определение альтернативного имени настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="8c68b-106">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="8c68b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c68b-107">Properties</span></span>
|<span data-ttu-id="8c68b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c68b-108">Property</span></span>|<span data-ttu-id="8c68b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8c68b-109">Type</span></span>|<span data-ttu-id="8c68b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c68b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c68b-111">Сантипе</span><span class="sxs-lookup"><span data-stu-id="8c68b-111">sanType</span></span>|[<span data-ttu-id="8c68b-112">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8c68b-112">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="8c68b-113">Настраиваемый тип SAN.</span><span class="sxs-lookup"><span data-stu-id="8c68b-113">Custom SAN Type.</span></span> <span data-ttu-id="8c68b-114">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="8c68b-114">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="8c68b-115">name</span><span class="sxs-lookup"><span data-stu-id="8c68b-115">name</span></span>|<span data-ttu-id="8c68b-116">String</span><span class="sxs-lookup"><span data-stu-id="8c68b-116">String</span></span>|<span data-ttu-id="8c68b-117">Настраиваемое имя сети хранения данных</span><span class="sxs-lookup"><span data-stu-id="8c68b-117">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c68b-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="8c68b-118">Relationships</span></span>
<span data-ttu-id="8c68b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8c68b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c68b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c68b-120">JSON Representation</span></span>
<span data-ttu-id="8c68b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c68b-121">Here is a JSON representation of the resource.</span></span>
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





