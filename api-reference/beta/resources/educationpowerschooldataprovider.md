---
title: ресурс Едукатионповерсчулдатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании PowerSchool в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 664b7c9c3ad255e502583fca6be332043e712a46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979618"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="8cc85-103">ресурс Едукатионповерсчулдатапровидер</span><span class="sxs-lookup"><span data-stu-id="8cc85-103">educationPowerSchoolDataProvider resource</span></span>

<span data-ttu-id="8cc85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc85-105">Используется для настройки профиля синхронизации данных School при использовании [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="8cc85-105">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="8cc85-106">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="8cc85-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8cc85-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cc85-107">Properties</span></span>

| <span data-ttu-id="8cc85-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cc85-108">Property</span></span>                       | <span data-ttu-id="8cc85-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8cc85-109">Type</span></span>                                     | <span data-ttu-id="8cc85-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8cc85-110">Description</span></span>                                                                            |
| :----------------------------- | :--------------------------------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="8cc85-111">алловтеачерсинмултиплесчулс</span><span class="sxs-lookup"><span data-stu-id="8cc85-111">allowTeachersInMultipleSchools</span></span> | <span data-ttu-id="8cc85-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-112">Boolean</span></span>                                  | <span data-ttu-id="8cc85-113">Указывает, содержит ли источник несколько идентификаторов для одного учащегося или преподавателя.</span><span class="sxs-lookup"><span data-stu-id="8cc85-113">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="8cc85-114">clientId</span><span class="sxs-lookup"><span data-stu-id="8cc85-114">clientId</span></span>                       | <span data-ttu-id="8cc85-115">String</span><span class="sxs-lookup"><span data-stu-id="8cc85-115">String</span></span>                                   | <span data-ttu-id="8cc85-116">Идентификатор клиента, используемый для подключения к PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="8cc85-116">The client ID used to connect to PowerSchool.</span></span>                                          |
| <span data-ttu-id="8cc85-117">clientSecret</span><span class="sxs-lookup"><span data-stu-id="8cc85-117">clientSecret</span></span>                   | <span data-ttu-id="8cc85-118">String</span><span class="sxs-lookup"><span data-stu-id="8cc85-118">String</span></span>                                   | <span data-ttu-id="8cc85-119">Секрет клиента для проверки подлинности подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="8cc85-119">The client secret to authenticate the connection to the PowerSchool instance.</span></span>          |
| <span data-ttu-id="8cc85-120">коннектионурл</span><span class="sxs-lookup"><span data-stu-id="8cc85-120">connectionUrl</span></span>                  | <span data-ttu-id="8cc85-121">String</span><span class="sxs-lookup"><span data-stu-id="8cc85-121">String</span></span>                                   | <span data-ttu-id="8cc85-122">URL-адрес подключения к экземпляру PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="8cc85-122">The connection URL to the PowerSchool instance.</span></span>                                        |
| <span data-ttu-id="8cc85-123">счулсидс</span><span class="sxs-lookup"><span data-stu-id="8cc85-123">schoolsIds</span></span>                     | <span data-ttu-id="8cc85-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8cc85-124">String collection</span></span>                        | <span data-ttu-id="8cc85-125">Список учебных заведений для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8cc85-125">The list of schools to sync.</span></span>                                                           |
| <span data-ttu-id="8cc85-126">счулеар</span><span class="sxs-lookup"><span data-stu-id="8cc85-126">schoolYear</span></span>                     | <span data-ttu-id="8cc85-127">String</span><span class="sxs-lookup"><span data-stu-id="8cc85-127">String</span></span>                                   | <span data-ttu-id="8cc85-128">Год учебного заведения для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8cc85-128">The school year to sync.</span></span>                                                               |
| <span data-ttu-id="8cc85-129">настроек</span><span class="sxs-lookup"><span data-stu-id="8cc85-129">customizations</span></span>                 | <span data-ttu-id="8cc85-130">[едукатионсинчронизатионкустомизатионс]</span><span class="sxs-lookup"><span data-stu-id="8cc85-130">[educationSynchronizationCustomizations]</span></span> | <span data-ttu-id="8cc85-131">Необязательная настройка, применяемая к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8cc85-131">Optional customization to be applied to the synchronization profile.</span></span>                   |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md
[едукатионсинчронизатионкустомизатионс]: educationsynchronizationcustomizations.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md

## <a name="json-representation"></a><span data-ttu-id="8cc85-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cc85-133">JSON representation</span></span>

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
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```


