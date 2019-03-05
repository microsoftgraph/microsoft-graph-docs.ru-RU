---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c321ea06e27e7d6fba0a35446e2b916aaf0689de
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253654"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="cc88c-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="cc88c-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="cc88c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc88c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc88c-105">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="cc88c-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="cc88c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc88c-106">Properties</span></span>
|<span data-ttu-id="cc88c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc88c-107">Property</span></span>|<span data-ttu-id="cc88c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cc88c-108">Type</span></span>|<span data-ttu-id="cc88c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cc88c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc88c-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="cc88c-110">subjectName</span></span>|<span data-ttu-id="cc88c-111">String</span><span class="sxs-lookup"><span data-stu-id="cc88c-111">String</span></span>|<span data-ttu-id="cc88c-112">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="cc88c-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="cc88c-113">description</span><span class="sxs-lookup"><span data-stu-id="cc88c-113">description</span></span>|<span data-ttu-id="cc88c-114">String</span><span class="sxs-lookup"><span data-stu-id="cc88c-114">String</span></span>|<span data-ttu-id="cc88c-115">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="cc88c-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="cc88c-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cc88c-116">expirationDateTime</span></span>|<span data-ttu-id="cc88c-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc88c-117">DateTimeOffset</span></span>|<span data-ttu-id="cc88c-118">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="cc88c-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="cc88c-119">certificate</span><span class="sxs-lookup"><span data-stu-id="cc88c-119">certificate</span></span>|<span data-ttu-id="cc88c-120">Двоичный</span><span class="sxs-lookup"><span data-stu-id="cc88c-120">Binary</span></span>|<span data-ttu-id="cc88c-121">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="cc88c-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc88c-122">Связи</span><span class="sxs-lookup"><span data-stu-id="cc88c-122">Relationships</span></span>
<span data-ttu-id="cc88c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="cc88c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc88c-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc88c-124">JSON Representation</span></span>
<span data-ttu-id="cc88c-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc88c-125">Here is a JSON representation of the resource.</span></span>
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



