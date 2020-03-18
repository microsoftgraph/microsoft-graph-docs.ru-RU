---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a08a4194fe06cbfe612d1127b28fd34c877da715
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780873"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="024c3-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="024c3-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="024c3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="024c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="024c3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="024c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="024c3-106">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="024c3-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="024c3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="024c3-107">Properties</span></span>
|<span data-ttu-id="024c3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="024c3-108">Property</span></span>|<span data-ttu-id="024c3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="024c3-109">Type</span></span>|<span data-ttu-id="024c3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="024c3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="024c3-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="024c3-111">subjectName</span></span>|<span data-ttu-id="024c3-112">String</span><span class="sxs-lookup"><span data-stu-id="024c3-112">String</span></span>|<span data-ttu-id="024c3-113">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="024c3-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="024c3-114">description</span><span class="sxs-lookup"><span data-stu-id="024c3-114">description</span></span>|<span data-ttu-id="024c3-115">String</span><span class="sxs-lookup"><span data-stu-id="024c3-115">String</span></span>|<span data-ttu-id="024c3-116">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="024c3-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="024c3-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="024c3-117">expirationDateTime</span></span>|<span data-ttu-id="024c3-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="024c3-118">DateTimeOffset</span></span>|<span data-ttu-id="024c3-119">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="024c3-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="024c3-120">certificate</span><span class="sxs-lookup"><span data-stu-id="024c3-120">certificate</span></span>|<span data-ttu-id="024c3-121">Двоичный</span><span class="sxs-lookup"><span data-stu-id="024c3-121">Binary</span></span>|<span data-ttu-id="024c3-122">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="024c3-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="024c3-123">Связи</span><span class="sxs-lookup"><span data-stu-id="024c3-123">Relationships</span></span>
<span data-ttu-id="024c3-124">Нет</span><span class="sxs-lookup"><span data-stu-id="024c3-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="024c3-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="024c3-125">JSON Representation</span></span>
<span data-ttu-id="024c3-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="024c3-126">Here is a JSON representation of the resource.</span></span>
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



