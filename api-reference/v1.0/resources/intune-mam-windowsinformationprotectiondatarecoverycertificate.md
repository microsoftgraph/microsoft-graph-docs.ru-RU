---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c321ea06e27e7d6fba0a35446e2b916aaf0689de
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561189"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="53b25-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="53b25-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="53b25-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53b25-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53b25-105">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="53b25-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="53b25-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="53b25-106">Properties</span></span>
|<span data-ttu-id="53b25-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="53b25-107">Property</span></span>|<span data-ttu-id="53b25-108">Тип</span><span class="sxs-lookup"><span data-stu-id="53b25-108">Type</span></span>|<span data-ttu-id="53b25-109">Описание</span><span class="sxs-lookup"><span data-stu-id="53b25-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b25-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="53b25-110">subjectName</span></span>|<span data-ttu-id="53b25-111">String</span><span class="sxs-lookup"><span data-stu-id="53b25-111">String</span></span>|<span data-ttu-id="53b25-112">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="53b25-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="53b25-113">description</span><span class="sxs-lookup"><span data-stu-id="53b25-113">description</span></span>|<span data-ttu-id="53b25-114">String</span><span class="sxs-lookup"><span data-stu-id="53b25-114">String</span></span>|<span data-ttu-id="53b25-115">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="53b25-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="53b25-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="53b25-116">expirationDateTime</span></span>|<span data-ttu-id="53b25-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53b25-117">DateTimeOffset</span></span>|<span data-ttu-id="53b25-118">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="53b25-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="53b25-119">certificate</span><span class="sxs-lookup"><span data-stu-id="53b25-119">certificate</span></span>|<span data-ttu-id="53b25-120">Двоичный</span><span class="sxs-lookup"><span data-stu-id="53b25-120">Binary</span></span>|<span data-ttu-id="53b25-121">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="53b25-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="53b25-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="53b25-122">Relationships</span></span>
<span data-ttu-id="53b25-123">Нет</span><span class="sxs-lookup"><span data-stu-id="53b25-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53b25-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53b25-124">JSON Representation</span></span>
<span data-ttu-id="53b25-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53b25-125">Here is a JSON representation of the resource.</span></span>
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



