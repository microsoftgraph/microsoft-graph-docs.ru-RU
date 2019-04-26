---
title: ресурс Едукатионповерсчулдатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании PowerSchool в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cee763995dd5a75b64d94e5f170d6fea992c20b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340579"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="04a45-103">ресурс Едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="04a45-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04a45-104">Используется для настройки профиля синхронизации данных School при использовании [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="04a45-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="04a45-105">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="04a45-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="04a45-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="04a45-106">Properties</span></span>

| <span data-ttu-id="04a45-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="04a45-107">Property</span></span> | <span data-ttu-id="04a45-108">Тип</span><span class="sxs-lookup"><span data-stu-id="04a45-108">Type</span></span> | <span data-ttu-id="04a45-109">Описание</span><span class="sxs-lookup"><span data-stu-id="04a45-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="04a45-110">**Коннектионурл**</span><span class="sxs-lookup"><span data-stu-id="04a45-110">**connectionUrl**</span></span> | <span data-ttu-id="04a45-111">String</span><span class="sxs-lookup"><span data-stu-id="04a45-111">String</span></span> | <span data-ttu-id="04a45-112">URL-адрес подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="04a45-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="04a45-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="04a45-113">**clientId**</span></span> | <span data-ttu-id="04a45-114">String</span><span class="sxs-lookup"><span data-stu-id="04a45-114">String</span></span> |  <span data-ttu-id="04a45-115">Идентификатор клиента, используемый для подключения к PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="04a45-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="04a45-116">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="04a45-116">**clientSecret**</span></span> | <span data-ttu-id="04a45-117">String</span><span class="sxs-lookup"><span data-stu-id="04a45-117">String</span></span> |  <span data-ttu-id="04a45-118">Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="04a45-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="04a45-119">**Счулсидс**</span><span class="sxs-lookup"><span data-stu-id="04a45-119">**schoolsIds**</span></span> | <span data-ttu-id="04a45-120">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04a45-120">String collection</span></span> |  <span data-ttu-id="04a45-121">Список учебных заведений для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="04a45-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="04a45-122">**Счулеар**</span><span class="sxs-lookup"><span data-stu-id="04a45-122">**schoolYear**</span></span> | <span data-ttu-id="04a45-123">String</span><span class="sxs-lookup"><span data-stu-id="04a45-123">String</span></span> |  <span data-ttu-id="04a45-124">Год учебного заведения для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="04a45-124">The school year to sync.</span></span> |
| <span data-ttu-id="04a45-125">**Алловтеачерсинмултиплесчулс**</span><span class="sxs-lookup"><span data-stu-id="04a45-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="04a45-126">Логический</span><span class="sxs-lookup"><span data-stu-id="04a45-126">Boolean</span></span> |  <span data-ttu-id="04a45-127">Указывает, содержит ли источник несколько идентификаторов для одного учащегося или преподавателя.</span><span class="sxs-lookup"><span data-stu-id="04a45-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="04a45-128">**настроек**</span><span class="sxs-lookup"><span data-stu-id="04a45-128">**customizations**</span></span> | [<span data-ttu-id="04a45-129">Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="04a45-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="04a45-130">НеОбязательная Настройка, применяемая к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="04a45-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04a45-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04a45-131">JSON representation</span></span>
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
  "schoolsIds": ["String"],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": "Boolean",
  "customizations": {"@odata.type": "microsoft.graph.educationSynchronizationCustomizations"}
}
```
