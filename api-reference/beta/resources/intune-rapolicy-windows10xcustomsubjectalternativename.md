---
title: Тип ресурса windows10XCustomSubjectAlternativeName
description: Тип базового профиля для сертификатов проверки подлинности (SCEP или PFX Create)
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 725d2cc13db1cb28b9286479f201b9bb38f6eefa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301912"
---
# <a name="windows10xcustomsubjectalternativename-resource-type"></a><span data-ttu-id="2537f-103">Тип ресурса windows10XCustomSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="2537f-103">windows10XCustomSubjectAlternativeName resource type</span></span>

<span data-ttu-id="2537f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2537f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2537f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2537f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2537f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2537f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2537f-107">Тип базового профиля для сертификатов проверки подлинности (SCEP или PFX Create)</span><span class="sxs-lookup"><span data-stu-id="2537f-107">Base Profile Type for Authentication Certificates (SCEP or PFX Create)</span></span>

## <a name="properties"></a><span data-ttu-id="2537f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2537f-108">Properties</span></span>
|<span data-ttu-id="2537f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2537f-109">Property</span></span>|<span data-ttu-id="2537f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2537f-110">Type</span></span>|<span data-ttu-id="2537f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2537f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2537f-112">сантипе</span><span class="sxs-lookup"><span data-stu-id="2537f-112">sanType</span></span>|[<span data-ttu-id="2537f-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2537f-113">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="2537f-114">Настраиваемый тип SAN.</span><span class="sxs-lookup"><span data-stu-id="2537f-114">Custom SAN Type.</span></span> <span data-ttu-id="2537f-115">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="2537f-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="2537f-116">name</span><span class="sxs-lookup"><span data-stu-id="2537f-116">name</span></span>|<span data-ttu-id="2537f-117">String</span><span class="sxs-lookup"><span data-stu-id="2537f-117">String</span></span>|<span data-ttu-id="2537f-118">Настраиваемое имя сети хранения данных</span><span class="sxs-lookup"><span data-stu-id="2537f-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="2537f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="2537f-119">Relationships</span></span>
<span data-ttu-id="2537f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2537f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2537f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2537f-121">JSON Representation</span></span>
<span data-ttu-id="2537f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2537f-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XCustomSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```




