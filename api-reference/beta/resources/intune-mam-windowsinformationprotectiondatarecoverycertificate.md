---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae0e8f6f09470d58669acb5123e25a13c6a51dd9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207262"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="bb51a-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="bb51a-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="bb51a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb51a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb51a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb51a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb51a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb51a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb51a-107">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="bb51a-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="bb51a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb51a-108">Properties</span></span>
|<span data-ttu-id="bb51a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb51a-109">Property</span></span>|<span data-ttu-id="bb51a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bb51a-110">Type</span></span>|<span data-ttu-id="bb51a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bb51a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb51a-112">subjectName</span><span class="sxs-lookup"><span data-stu-id="bb51a-112">subjectName</span></span>|<span data-ttu-id="bb51a-113">String</span><span class="sxs-lookup"><span data-stu-id="bb51a-113">String</span></span>|<span data-ttu-id="bb51a-114">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="bb51a-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="bb51a-115">description</span><span class="sxs-lookup"><span data-stu-id="bb51a-115">description</span></span>|<span data-ttu-id="bb51a-116">String</span><span class="sxs-lookup"><span data-stu-id="bb51a-116">String</span></span>|<span data-ttu-id="bb51a-117">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="bb51a-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="bb51a-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bb51a-118">expirationDateTime</span></span>|<span data-ttu-id="bb51a-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb51a-119">DateTimeOffset</span></span>|<span data-ttu-id="bb51a-120">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="bb51a-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="bb51a-121">certificate</span><span class="sxs-lookup"><span data-stu-id="bb51a-121">certificate</span></span>|<span data-ttu-id="bb51a-122">Двоичный</span><span class="sxs-lookup"><span data-stu-id="bb51a-122">Binary</span></span>|<span data-ttu-id="bb51a-123">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="bb51a-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb51a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="bb51a-124">Relationships</span></span>
<span data-ttu-id="bb51a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="bb51a-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb51a-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb51a-126">JSON Representation</span></span>
<span data-ttu-id="bb51a-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb51a-127">Here is a JSON representation of the resource.</span></span>
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




