---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dcdd83346072a6f2946060a68064989b44ca3eb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940605"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="4e988-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4e988-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="4e988-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e988-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e988-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e988-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e988-106">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="4e988-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="4e988-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e988-107">Properties</span></span>
|<span data-ttu-id="4e988-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e988-108">Property</span></span>|<span data-ttu-id="4e988-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4e988-109">Type</span></span>|<span data-ttu-id="4e988-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4e988-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e988-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="4e988-111">subjectName</span></span>|<span data-ttu-id="4e988-112">String</span><span class="sxs-lookup"><span data-stu-id="4e988-112">String</span></span>|<span data-ttu-id="4e988-113">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="4e988-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="4e988-114">description</span><span class="sxs-lookup"><span data-stu-id="4e988-114">description</span></span>|<span data-ttu-id="4e988-115">String</span><span class="sxs-lookup"><span data-stu-id="4e988-115">String</span></span>|<span data-ttu-id="4e988-116">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="4e988-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="4e988-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4e988-117">expirationDateTime</span></span>|<span data-ttu-id="4e988-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e988-118">DateTimeOffset</span></span>|<span data-ttu-id="4e988-119">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="4e988-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="4e988-120">certificate</span><span class="sxs-lookup"><span data-stu-id="4e988-120">certificate</span></span>|<span data-ttu-id="4e988-121">Двоичный</span><span class="sxs-lookup"><span data-stu-id="4e988-121">Binary</span></span>|<span data-ttu-id="4e988-122">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="4e988-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e988-123">Связи</span><span class="sxs-lookup"><span data-stu-id="4e988-123">Relationships</span></span>
<span data-ttu-id="4e988-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4e988-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e988-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e988-125">JSON Representation</span></span>
<span data-ttu-id="4e988-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e988-126">Here is a JSON representation of the resource.</span></span>
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




