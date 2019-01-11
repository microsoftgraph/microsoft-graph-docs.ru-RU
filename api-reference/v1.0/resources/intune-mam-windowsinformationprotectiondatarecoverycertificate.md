---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 72edbdc16b2d84a2df6a4582bba12bab2feaa04c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821065"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="a2f61-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a2f61-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="a2f61-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a2f61-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2f61-105">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="a2f61-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="a2f61-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2f61-106">Properties</span></span>
|<span data-ttu-id="a2f61-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2f61-107">Property</span></span>|<span data-ttu-id="a2f61-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a2f61-108">Type</span></span>|<span data-ttu-id="a2f61-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a2f61-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2f61-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="a2f61-110">subjectName</span></span>|<span data-ttu-id="a2f61-111">String</span><span class="sxs-lookup"><span data-stu-id="a2f61-111">String</span></span>|<span data-ttu-id="a2f61-112">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="a2f61-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="a2f61-113">описание</span><span class="sxs-lookup"><span data-stu-id="a2f61-113">description</span></span>|<span data-ttu-id="a2f61-114">String</span><span class="sxs-lookup"><span data-stu-id="a2f61-114">String</span></span>|<span data-ttu-id="a2f61-115">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="a2f61-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="a2f61-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a2f61-116">expirationDateTime</span></span>|<span data-ttu-id="a2f61-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2f61-117">DateTimeOffset</span></span>|<span data-ttu-id="a2f61-118">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="a2f61-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="a2f61-119">certificate</span><span class="sxs-lookup"><span data-stu-id="a2f61-119">certificate</span></span>|<span data-ttu-id="a2f61-120">Двоичный</span><span class="sxs-lookup"><span data-stu-id="a2f61-120">Binary</span></span>|<span data-ttu-id="a2f61-121">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="a2f61-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2f61-122">Связи</span><span class="sxs-lookup"><span data-stu-id="a2f61-122">Relationships</span></span>
<span data-ttu-id="a2f61-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a2f61-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a2f61-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2f61-124">JSON Representation</span></span>
<span data-ttu-id="a2f61-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2f61-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



