---
title: ресурс Едукатионповерсчулдатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании PowerSchool в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4fda7cc98c8041aad45a0ef8453affc9af34edc5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501229"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="04293-103">ресурс Едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="04293-103">educationPowerSchoolDataProvider resource</span></span>

<span data-ttu-id="04293-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04293-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04293-105">Используется для настройки профиля синхронизации данных School при использовании [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="04293-105">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="04293-106">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="04293-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="04293-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="04293-107">Properties</span></span>

| <span data-ttu-id="04293-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="04293-108">Property</span></span> | <span data-ttu-id="04293-109">Тип</span><span class="sxs-lookup"><span data-stu-id="04293-109">Type</span></span> | <span data-ttu-id="04293-110">Описание</span><span class="sxs-lookup"><span data-stu-id="04293-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="04293-111">**коннектионурл**</span><span class="sxs-lookup"><span data-stu-id="04293-111">**connectionUrl**</span></span> | <span data-ttu-id="04293-112">String</span><span class="sxs-lookup"><span data-stu-id="04293-112">String</span></span> | <span data-ttu-id="04293-113">URL-адрес подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="04293-113">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="04293-114">**clientId**</span><span class="sxs-lookup"><span data-stu-id="04293-114">**clientId**</span></span> | <span data-ttu-id="04293-115">String</span><span class="sxs-lookup"><span data-stu-id="04293-115">String</span></span> |  <span data-ttu-id="04293-116">Идентификатор клиента, используемый для подключения к PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="04293-116">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="04293-117">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="04293-117">**clientSecret**</span></span> | <span data-ttu-id="04293-118">String</span><span class="sxs-lookup"><span data-stu-id="04293-118">String</span></span> |  <span data-ttu-id="04293-119">Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="04293-119">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="04293-120">**счулсидс**</span><span class="sxs-lookup"><span data-stu-id="04293-120">**schoolsIds**</span></span> | <span data-ttu-id="04293-121">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04293-121">String collection</span></span> |  <span data-ttu-id="04293-122">Список учебных заведений для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="04293-122">The list of schools to sync.</span></span> |
| <span data-ttu-id="04293-123">**счулеар**</span><span class="sxs-lookup"><span data-stu-id="04293-123">**schoolYear**</span></span> | <span data-ttu-id="04293-124">String</span><span class="sxs-lookup"><span data-stu-id="04293-124">String</span></span> |  <span data-ttu-id="04293-125">Год учебного заведения для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="04293-125">The school year to sync.</span></span> |
| <span data-ttu-id="04293-126">**алловтеачерсинмултиплесчулс**</span><span class="sxs-lookup"><span data-stu-id="04293-126">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="04293-127">Логический</span><span class="sxs-lookup"><span data-stu-id="04293-127">Boolean</span></span> |  <span data-ttu-id="04293-128">Указывает, содержит ли источник несколько идентификаторов для одного учащегося или преподавателя.</span><span class="sxs-lookup"><span data-stu-id="04293-128">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="04293-129">**настроек**</span><span class="sxs-lookup"><span data-stu-id="04293-129">**customizations**</span></span> | [<span data-ttu-id="04293-130">едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="04293-130">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="04293-131">Необязательная настройка, применяемая к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="04293-131">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04293-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04293-132">JSON representation</span></span>
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
