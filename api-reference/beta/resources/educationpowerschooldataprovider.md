---
title: ресурс Едукатионповерсчулдатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании PowerSchool в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6a036435cb7cc1a4ef70960b09feb600fe7f39f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972599"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="02a93-103">ресурс Едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="02a93-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02a93-104">Используется для настройки профиля синхронизации данных School при использовании [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="02a93-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="02a93-105">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="02a93-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="02a93-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="02a93-106">Properties</span></span>

| <span data-ttu-id="02a93-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="02a93-107">Property</span></span> | <span data-ttu-id="02a93-108">Тип</span><span class="sxs-lookup"><span data-stu-id="02a93-108">Type</span></span> | <span data-ttu-id="02a93-109">Описание</span><span class="sxs-lookup"><span data-stu-id="02a93-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="02a93-110">**Коннектионурл**</span><span class="sxs-lookup"><span data-stu-id="02a93-110">**connectionUrl**</span></span> | <span data-ttu-id="02a93-111">String</span><span class="sxs-lookup"><span data-stu-id="02a93-111">String</span></span> | <span data-ttu-id="02a93-112">URL-адрес подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="02a93-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="02a93-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="02a93-113">**clientId**</span></span> | <span data-ttu-id="02a93-114">String</span><span class="sxs-lookup"><span data-stu-id="02a93-114">String</span></span> |  <span data-ttu-id="02a93-115">Идентификатор клиента, используемый для подключения к PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="02a93-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="02a93-116">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="02a93-116">**clientSecret**</span></span> | <span data-ttu-id="02a93-117">String</span><span class="sxs-lookup"><span data-stu-id="02a93-117">String</span></span> |  <span data-ttu-id="02a93-118">Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="02a93-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="02a93-119">**Счулсидс**</span><span class="sxs-lookup"><span data-stu-id="02a93-119">**schoolsIds**</span></span> | <span data-ttu-id="02a93-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="02a93-120">String collection</span></span> |  <span data-ttu-id="02a93-121">Список учебных заведений для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="02a93-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="02a93-122">**Счулеар**</span><span class="sxs-lookup"><span data-stu-id="02a93-122">**schoolYear**</span></span> | <span data-ttu-id="02a93-123">String</span><span class="sxs-lookup"><span data-stu-id="02a93-123">String</span></span> |  <span data-ttu-id="02a93-124">Год учебного заведения для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="02a93-124">The school year to sync.</span></span> |
| <span data-ttu-id="02a93-125">**Алловтеачерсинмултиплесчулс**</span><span class="sxs-lookup"><span data-stu-id="02a93-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="02a93-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="02a93-126">Boolean</span></span> |  <span data-ttu-id="02a93-127">Указывает, содержит ли источник несколько идентификаторов для одного учащегося или преподавателя.</span><span class="sxs-lookup"><span data-stu-id="02a93-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="02a93-128">**настроек**</span><span class="sxs-lookup"><span data-stu-id="02a93-128">**customizations**</span></span> | [<span data-ttu-id="02a93-129">Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="02a93-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="02a93-130">Необязательная настройка, применяемая к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="02a93-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02a93-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02a93-131">JSON representation</span></span>
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
