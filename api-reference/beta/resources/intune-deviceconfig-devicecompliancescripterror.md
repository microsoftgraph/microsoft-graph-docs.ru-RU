---
title: Тип ресурса Девицекомплианцескриптеррор
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd8a801d34bb5a7ad07c7e769d25fa0a05e31a53
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260260"
---
# <a name="devicecompliancescripterror-resource-type"></a><span data-ttu-id="978ae-103">Тип ресурса Девицекомплианцескриптеррор</span><span class="sxs-lookup"><span data-stu-id="978ae-103">deviceComplianceScriptError resource type</span></span>

<span data-ttu-id="978ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="978ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="978ae-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="978ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="978ae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="978ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="978ae-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="978ae-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="978ae-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="978ae-108">Properties</span></span>
|<span data-ttu-id="978ae-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="978ae-109">Property</span></span>|<span data-ttu-id="978ae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="978ae-110">Type</span></span>|<span data-ttu-id="978ae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="978ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="978ae-112">code</span><span class="sxs-lookup"><span data-stu-id="978ae-112">code</span></span>|[<span data-ttu-id="978ae-113">code</span><span class="sxs-lookup"><span data-stu-id="978ae-113">code</span></span>](../resources/intune-deviceconfig-code.md)|<span data-ttu-id="978ae-114">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="978ae-114">Error code.</span></span> <span data-ttu-id="978ae-115">Допустимые значения:,,,,,,,,,,, `none` `jsonFileInvalid` `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` , `moreInfoUriInvalid` , `moreInfoUriTooLarge` , `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` ,,,,,,,,,,,,,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="978ae-115">Possible values are: `none`, `jsonFileInvalid`, `jsonFileMissing`, `jsonFileTooLarge`, `rulesMissing`, `duplicateRules`, `tooManyRulesSpecified`, `operatorMissing`, `operatorNotSupported`, `datatypeMissing`, `datatypeNotSupported`, `operatorDataTypeCombinationNotSupported`, `moreInfoUriMissing`, `moreInfoUriInvalid`, `moreInfoUriTooLarge`, `descriptionMissing`, `descriptionInvalid`, `descriptionTooLarge`, `titleMissing`, `titleInvalid`, `titleTooLarge`, `operandMissing`, `operandInvalid`, `operandTooLarge`, `settingNameMissing`, `settingNameInvalid`, `settingNameTooLarge`, `englishLocaleMissing`, `duplicateLocales`, `unrecognizedLocale`, `unknown`, `remediationStringsMissing`.</span></span>|
|<span data-ttu-id="978ae-116">message</span><span class="sxs-lookup"><span data-stu-id="978ae-116">message</span></span>|<span data-ttu-id="978ae-117">String</span><span class="sxs-lookup"><span data-stu-id="978ae-117">String</span></span>|<span data-ttu-id="978ae-118">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="978ae-118">Error message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="978ae-119">Связи</span><span class="sxs-lookup"><span data-stu-id="978ae-119">Relationships</span></span>
<span data-ttu-id="978ae-120">Нет</span><span class="sxs-lookup"><span data-stu-id="978ae-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="978ae-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="978ae-121">JSON Representation</span></span>
<span data-ttu-id="978ae-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="978ae-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptError",
  "code": "String",
  "message": "String"
}
```




