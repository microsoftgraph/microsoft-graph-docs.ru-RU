---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a23a05a53170929712d4cfd8c4dd9f634fba5dc4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751281"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="97dcc-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="97dcc-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="97dcc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97dcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97dcc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97dcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97dcc-106">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="97dcc-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="97dcc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="97dcc-107">Properties</span></span>
|<span data-ttu-id="97dcc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="97dcc-108">Property</span></span>|<span data-ttu-id="97dcc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="97dcc-109">Type</span></span>|<span data-ttu-id="97dcc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="97dcc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97dcc-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="97dcc-111">subjectName</span></span>|<span data-ttu-id="97dcc-112">String</span><span class="sxs-lookup"><span data-stu-id="97dcc-112">String</span></span>|<span data-ttu-id="97dcc-113">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="97dcc-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="97dcc-114">description</span><span class="sxs-lookup"><span data-stu-id="97dcc-114">description</span></span>|<span data-ttu-id="97dcc-115">String</span><span class="sxs-lookup"><span data-stu-id="97dcc-115">String</span></span>|<span data-ttu-id="97dcc-116">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="97dcc-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="97dcc-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="97dcc-117">expirationDateTime</span></span>|<span data-ttu-id="97dcc-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97dcc-118">DateTimeOffset</span></span>|<span data-ttu-id="97dcc-119">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="97dcc-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="97dcc-120">certificate</span><span class="sxs-lookup"><span data-stu-id="97dcc-120">certificate</span></span>|<span data-ttu-id="97dcc-121">Двоичный</span><span class="sxs-lookup"><span data-stu-id="97dcc-121">Binary</span></span>|<span data-ttu-id="97dcc-122">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="97dcc-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="97dcc-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="97dcc-123">Relationships</span></span>
<span data-ttu-id="97dcc-124">Нет</span><span class="sxs-lookup"><span data-stu-id="97dcc-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97dcc-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97dcc-125">JSON Representation</span></span>
<span data-ttu-id="97dcc-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97dcc-126">Here is a JSON representation of the resource.</span></span>
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




