---
title: ресурс Едукатионповерсчулдатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании PowerSchool в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507128"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="39afe-103">ресурс Едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="39afe-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39afe-104">Используется для настройки профиля синхронизации данных School при использовании [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="39afe-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="39afe-105">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="39afe-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="39afe-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="39afe-106">Properties</span></span>

| <span data-ttu-id="39afe-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="39afe-107">Property</span></span> | <span data-ttu-id="39afe-108">Тип</span><span class="sxs-lookup"><span data-stu-id="39afe-108">Type</span></span> | <span data-ttu-id="39afe-109">Описание</span><span class="sxs-lookup"><span data-stu-id="39afe-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="39afe-110">**Коннектионурл**</span><span class="sxs-lookup"><span data-stu-id="39afe-110">**connectionUrl**</span></span> | <span data-ttu-id="39afe-111">String</span><span class="sxs-lookup"><span data-stu-id="39afe-111">String</span></span> | <span data-ttu-id="39afe-112">URL-адрес подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="39afe-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="39afe-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="39afe-113">**clientId**</span></span> | <span data-ttu-id="39afe-114">String</span><span class="sxs-lookup"><span data-stu-id="39afe-114">String</span></span> |  <span data-ttu-id="39afe-115">Идентификатор клиента, используемый для подключения к PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="39afe-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="39afe-116">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="39afe-116">**clientSecret**</span></span> | <span data-ttu-id="39afe-117">String</span><span class="sxs-lookup"><span data-stu-id="39afe-117">String</span></span> |  <span data-ttu-id="39afe-118">Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="39afe-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="39afe-119">**Счулсидс**</span><span class="sxs-lookup"><span data-stu-id="39afe-119">**schoolsIds**</span></span> | <span data-ttu-id="39afe-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="39afe-120">String collection</span></span> |  <span data-ttu-id="39afe-121">Список учебных заведений для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="39afe-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="39afe-122">**Счулеар**</span><span class="sxs-lookup"><span data-stu-id="39afe-122">**schoolYear**</span></span> | <span data-ttu-id="39afe-123">String</span><span class="sxs-lookup"><span data-stu-id="39afe-123">String</span></span> |  <span data-ttu-id="39afe-124">Год учебного заведения для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="39afe-124">The school year to sync.</span></span> |
| <span data-ttu-id="39afe-125">**Алловтеачерсинмултиплесчулс**</span><span class="sxs-lookup"><span data-stu-id="39afe-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="39afe-126">Логический</span><span class="sxs-lookup"><span data-stu-id="39afe-126">Boolean</span></span> |  <span data-ttu-id="39afe-127">Указывает, содержит ли источник несколько идентификаторов для одного учащегося или преподавателя.</span><span class="sxs-lookup"><span data-stu-id="39afe-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="39afe-128">**настроек**</span><span class="sxs-lookup"><span data-stu-id="39afe-128">**customizations**</span></span> | [<span data-ttu-id="39afe-129">Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="39afe-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="39afe-130">НеОбязательная Настройка, применяемая к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="39afe-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39afe-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39afe-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerschooldataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
