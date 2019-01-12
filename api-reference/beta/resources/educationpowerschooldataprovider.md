---
title: educationPowerSchoolDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при PowerSchool используется в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a22c3cf68a4a5b4c12dc4e7105f17eed4fc006f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982759"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="e4dd7-103">educationPowerSchoolDataProvider ресурсов</span><span class="sxs-lookup"><span data-stu-id="e4dd7-103">educationPowerSchoolDataProvider resource</span></span>

> <span data-ttu-id="e4dd7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e4dd7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4dd7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4dd7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4dd7-106">Используется для настройки синхронизации профилей данных school при [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) используется в качестве источника ввода.</span><span class="sxs-lookup"><span data-stu-id="e4dd7-106">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="e4dd7-107">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="e4dd7-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e4dd7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4dd7-108">Properties</span></span>

| <span data-ttu-id="e4dd7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4dd7-109">Property</span></span> | <span data-ttu-id="e4dd7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e4dd7-110">Type</span></span> | <span data-ttu-id="e4dd7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e4dd7-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="e4dd7-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="e4dd7-112">**connectionUrl**</span></span> | <span data-ttu-id="e4dd7-113">String</span><span class="sxs-lookup"><span data-stu-id="e4dd7-113">String</span></span> | <span data-ttu-id="e4dd7-114">URL-адрес подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="e4dd7-114">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="e4dd7-115">**clientId**</span><span class="sxs-lookup"><span data-stu-id="e4dd7-115">**clientId**</span></span> | <span data-ttu-id="e4dd7-116">String</span><span class="sxs-lookup"><span data-stu-id="e4dd7-116">String</span></span> |  <span data-ttu-id="e4dd7-117">Идентификатор клиента, используемого для подключения к PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="e4dd7-117">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="e4dd7-118">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="e4dd7-118">**clientSecret**</span></span> | <span data-ttu-id="e4dd7-119">String</span><span class="sxs-lookup"><span data-stu-id="e4dd7-119">String</span></span> |  <span data-ttu-id="e4dd7-120">Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="e4dd7-120">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="e4dd7-121">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="e4dd7-121">**schoolsIds**</span></span> | <span data-ttu-id="e4dd7-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e4dd7-122">String collection</span></span> |  <span data-ttu-id="e4dd7-123">Список школы для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e4dd7-123">The list of schools to sync.</span></span> |
| <span data-ttu-id="e4dd7-124">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="e4dd7-124">**schoolYear**</span></span> | <span data-ttu-id="e4dd7-125">String</span><span class="sxs-lookup"><span data-stu-id="e4dd7-125">String</span></span> |  <span data-ttu-id="e4dd7-126">Учебный год для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e4dd7-126">The school year to sync.</span></span> |
| <span data-ttu-id="e4dd7-127">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="e4dd7-127">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="e4dd7-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4dd7-128">Boolean</span></span> |  <span data-ttu-id="e4dd7-129">Указывает, имеет ли источник несколько идентификаторов для одного студент и преподаватель.</span><span class="sxs-lookup"><span data-stu-id="e4dd7-129">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="e4dd7-130">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="e4dd7-130">**customizations**</span></span> | [<span data-ttu-id="e4dd7-131">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="e4dd7-131">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="e4dd7-132">Дополнительные настройки применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="e4dd7-132">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4dd7-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4dd7-133">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
