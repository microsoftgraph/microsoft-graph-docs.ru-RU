---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: tfitzmac
ms.openlocfilehash: c45abb14669c3cf67571748a9da7d62bed037ff6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325825"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="d7fc1-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d7fc1-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="d7fc1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7fc1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7fc1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7fc1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7fc1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d7fc1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7fc1-107">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="d7fc1-107">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="d7fc1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7fc1-108">Properties</span></span>
|<span data-ttu-id="d7fc1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7fc1-109">Property</span></span>|<span data-ttu-id="d7fc1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d7fc1-110">Type</span></span>|<span data-ttu-id="d7fc1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7fc1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7fc1-112">subjectName</span><span class="sxs-lookup"><span data-stu-id="d7fc1-112">subjectName</span></span>|<span data-ttu-id="d7fc1-113">String</span><span class="sxs-lookup"><span data-stu-id="d7fc1-113">String</span></span>|<span data-ttu-id="d7fc1-114">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="d7fc1-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="d7fc1-115">описание</span><span class="sxs-lookup"><span data-stu-id="d7fc1-115">description</span></span>|<span data-ttu-id="d7fc1-116">String</span><span class="sxs-lookup"><span data-stu-id="d7fc1-116">String</span></span>|<span data-ttu-id="d7fc1-117">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="d7fc1-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="d7fc1-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d7fc1-118">expirationDateTime</span></span>|<span data-ttu-id="d7fc1-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7fc1-119">DateTimeOffset</span></span>|<span data-ttu-id="d7fc1-120">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="d7fc1-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="d7fc1-121">certificate</span><span class="sxs-lookup"><span data-stu-id="d7fc1-121">certificate</span></span>|<span data-ttu-id="d7fc1-122">Двоичный</span><span class="sxs-lookup"><span data-stu-id="d7fc1-122">Binary</span></span>|<span data-ttu-id="d7fc1-123">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="d7fc1-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7fc1-124">Связи</span><span class="sxs-lookup"><span data-stu-id="d7fc1-124">Relationships</span></span>
<span data-ttu-id="d7fc1-125">Нет</span><span class="sxs-lookup"><span data-stu-id="d7fc1-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d7fc1-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7fc1-126">JSON Representation</span></span>
<span data-ttu-id="d7fc1-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7fc1-127">Here is a JSON representation of the resource.</span></span>
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





