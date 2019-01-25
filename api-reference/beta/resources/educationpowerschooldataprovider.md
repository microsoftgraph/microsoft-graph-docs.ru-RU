---
title: educationPowerSchoolDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при PowerSchool используется в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510465"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="2e0fe-103">educationPowerSchoolDataProvider ресурсов</span><span class="sxs-lookup"><span data-stu-id="2e0fe-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e0fe-104">Используется для настройки синхронизации профилей данных school при [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) используется в качестве источника ввода.</span><span class="sxs-lookup"><span data-stu-id="2e0fe-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="2e0fe-105">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="2e0fe-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2e0fe-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e0fe-106">Properties</span></span>

| <span data-ttu-id="2e0fe-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e0fe-107">Property</span></span> | <span data-ttu-id="2e0fe-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2e0fe-108">Type</span></span> | <span data-ttu-id="2e0fe-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2e0fe-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2e0fe-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="2e0fe-110">**connectionUrl**</span></span> | <span data-ttu-id="2e0fe-111">String</span><span class="sxs-lookup"><span data-stu-id="2e0fe-111">String</span></span> | <span data-ttu-id="2e0fe-112">URL-адрес подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="2e0fe-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="2e0fe-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="2e0fe-113">**clientId**</span></span> | <span data-ttu-id="2e0fe-114">String</span><span class="sxs-lookup"><span data-stu-id="2e0fe-114">String</span></span> |  <span data-ttu-id="2e0fe-115">Идентификатор клиента, используемого для подключения к PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="2e0fe-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="2e0fe-116">client_secret</span><span class="sxs-lookup"><span data-stu-id="2e0fe-116">**clientSecret**</span></span> | <span data-ttu-id="2e0fe-117">String</span><span class="sxs-lookup"><span data-stu-id="2e0fe-117">String</span></span> |  <span data-ttu-id="2e0fe-118">Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="2e0fe-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="2e0fe-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="2e0fe-119">**schoolsIds**</span></span> | <span data-ttu-id="2e0fe-120">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2e0fe-120">String collection</span></span> |  <span data-ttu-id="2e0fe-121">Список школы для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2e0fe-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="2e0fe-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="2e0fe-122">**schoolYear**</span></span> | <span data-ttu-id="2e0fe-123">String</span><span class="sxs-lookup"><span data-stu-id="2e0fe-123">String</span></span> |  <span data-ttu-id="2e0fe-124">Учебный год для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2e0fe-124">The school year to sync.</span></span> |
| <span data-ttu-id="2e0fe-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="2e0fe-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="2e0fe-126">Логическое</span><span class="sxs-lookup"><span data-stu-id="2e0fe-126">Boolean</span></span> |  <span data-ttu-id="2e0fe-127">Указывает, имеет ли источник несколько идентификаторов для одного студент и преподаватель.</span><span class="sxs-lookup"><span data-stu-id="2e0fe-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="2e0fe-128">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="2e0fe-128">**customizations**</span></span> | [<span data-ttu-id="2e0fe-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="2e0fe-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="2e0fe-130">Дополнительные настройки применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="2e0fe-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e0fe-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e0fe-131">JSON representation</span></span>
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
