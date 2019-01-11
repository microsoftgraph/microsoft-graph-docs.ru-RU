---
title: educationPowerSchoolDataProvider ресурсов
description: Используется для настройки синхронизации профилей данных school при PowerSchool используется в качестве источника ввода.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 48a23a2e2a50e2e235b5722466c67094275236a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868784"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="b2b9a-103">educationPowerSchoolDataProvider ресурсов</span><span class="sxs-lookup"><span data-stu-id="b2b9a-103">educationPowerSchoolDataProvider resource</span></span>

> <span data-ttu-id="b2b9a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2b9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2b9a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2b9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2b9a-106">Используется для настройки синхронизации профилей данных school при [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) используется в качестве источника ввода.</span><span class="sxs-lookup"><span data-stu-id="b2b9a-106">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="b2b9a-107">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="b2b9a-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b2b9a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2b9a-108">Properties</span></span>

| <span data-ttu-id="b2b9a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2b9a-109">Property</span></span> | <span data-ttu-id="b2b9a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b2b9a-110">Type</span></span> | <span data-ttu-id="b2b9a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2b9a-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b2b9a-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="b2b9a-112">**connectionUrl**</span></span> | <span data-ttu-id="b2b9a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b2b9a-113">String</span></span> | <span data-ttu-id="b2b9a-114">URL-адрес подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="b2b9a-114">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="b2b9a-115">**clientId**</span><span class="sxs-lookup"><span data-stu-id="b2b9a-115">**clientId**</span></span> | <span data-ttu-id="b2b9a-116">Строка</span><span class="sxs-lookup"><span data-stu-id="b2b9a-116">String</span></span> |  <span data-ttu-id="b2b9a-117">Идентификатор клиента, используемого для подключения к PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="b2b9a-117">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="b2b9a-118">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="b2b9a-118">**clientSecret**</span></span> | <span data-ttu-id="b2b9a-119">Строка</span><span class="sxs-lookup"><span data-stu-id="b2b9a-119">String</span></span> |  <span data-ttu-id="b2b9a-120">Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="b2b9a-120">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="b2b9a-121">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="b2b9a-121">**schoolsIds**</span></span> | <span data-ttu-id="b2b9a-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b2b9a-122">String collection</span></span> |  <span data-ttu-id="b2b9a-123">Список школы для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b2b9a-123">The list of schools to sync.</span></span> |
| <span data-ttu-id="b2b9a-124">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="b2b9a-124">**schoolYear**</span></span> | <span data-ttu-id="b2b9a-125">Строка</span><span class="sxs-lookup"><span data-stu-id="b2b9a-125">String</span></span> |  <span data-ttu-id="b2b9a-126">Учебный год для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b2b9a-126">The school year to sync.</span></span> |
| <span data-ttu-id="b2b9a-127">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="b2b9a-127">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="b2b9a-128">Логический</span><span class="sxs-lookup"><span data-stu-id="b2b9a-128">Boolean</span></span> |  <span data-ttu-id="b2b9a-129">Указывает, имеет ли источник несколько идентификаторов для одного студент и преподаватель.</span><span class="sxs-lookup"><span data-stu-id="b2b9a-129">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="b2b9a-130">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="b2b9a-130">**customizations**</span></span> | [<span data-ttu-id="b2b9a-131">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="b2b9a-131">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="b2b9a-132">Дополнительные настройки применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="b2b9a-132">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2b9a-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2b9a-133">JSON representation</span></span>
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
