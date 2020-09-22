---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1da5da59fb0b3b2485ed2dd22710e13f64307843
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984378"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="8ca03-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8ca03-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="8ca03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ca03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ca03-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ca03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ca03-106">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="8ca03-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="8ca03-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ca03-107">Properties</span></span>
|<span data-ttu-id="8ca03-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ca03-108">Property</span></span>|<span data-ttu-id="8ca03-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8ca03-109">Type</span></span>|<span data-ttu-id="8ca03-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8ca03-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ca03-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="8ca03-111">subjectName</span></span>|<span data-ttu-id="8ca03-112">String</span><span class="sxs-lookup"><span data-stu-id="8ca03-112">String</span></span>|<span data-ttu-id="8ca03-113">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8ca03-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="8ca03-114">description</span><span class="sxs-lookup"><span data-stu-id="8ca03-114">description</span></span>|<span data-ttu-id="8ca03-115">String</span><span class="sxs-lookup"><span data-stu-id="8ca03-115">String</span></span>|<span data-ttu-id="8ca03-116">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8ca03-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="8ca03-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8ca03-117">expirationDateTime</span></span>|<span data-ttu-id="8ca03-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ca03-118">DateTimeOffset</span></span>|<span data-ttu-id="8ca03-119">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8ca03-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="8ca03-120">certificate</span><span class="sxs-lookup"><span data-stu-id="8ca03-120">certificate</span></span>|<span data-ttu-id="8ca03-121">Двоичный</span><span class="sxs-lookup"><span data-stu-id="8ca03-121">Binary</span></span>|<span data-ttu-id="8ca03-122">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8ca03-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ca03-123">Связи</span><span class="sxs-lookup"><span data-stu-id="8ca03-123">Relationships</span></span>
<span data-ttu-id="8ca03-124">Нет</span><span class="sxs-lookup"><span data-stu-id="8ca03-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ca03-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ca03-125">JSON Representation</span></span>
<span data-ttu-id="8ca03-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ca03-126">Here is a JSON representation of the resource.</span></span>
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









