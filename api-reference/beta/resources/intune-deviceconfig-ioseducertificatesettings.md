---
title: Тип ресурса Иоседуцертификатесеттингс
description: Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd063ec70dd794ffb151036ea7bbbda090829343
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001259"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="29c62-103">Тип ресурса Иоседуцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="29c62-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="29c62-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29c62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29c62-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="29c62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29c62-106">Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="29c62-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="29c62-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="29c62-107">Properties</span></span>
|<span data-ttu-id="29c62-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="29c62-108">Property</span></span>|<span data-ttu-id="29c62-109">Тип</span><span class="sxs-lookup"><span data-stu-id="29c62-109">Type</span></span>|<span data-ttu-id="29c62-110">Описание</span><span class="sxs-lookup"><span data-stu-id="29c62-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29c62-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="29c62-111">trustedRootCertificate</span></span>|<span data-ttu-id="29c62-112">Binary</span><span class="sxs-lookup"><span data-stu-id="29c62-112">Binary</span></span>|<span data-ttu-id="29c62-113">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="29c62-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="29c62-114">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="29c62-114">certFileName</span></span>|<span data-ttu-id="29c62-115">String</span><span class="sxs-lookup"><span data-stu-id="29c62-115">String</span></span>|<span data-ttu-id="29c62-116">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="29c62-116">File name to display in UI.</span></span>|
|<span data-ttu-id="29c62-117">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="29c62-117">certificationAuthority</span></span>|<span data-ttu-id="29c62-118">String</span><span class="sxs-lookup"><span data-stu-id="29c62-118">String</span></span>|<span data-ttu-id="29c62-119">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="29c62-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="29c62-120">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="29c62-120">certificationAuthorityName</span></span>|<span data-ttu-id="29c62-121">String</span><span class="sxs-lookup"><span data-stu-id="29c62-121">String</span></span>|<span data-ttu-id="29c62-122">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="29c62-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="29c62-123">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="29c62-123">certificateTemplateName</span></span>|<span data-ttu-id="29c62-124">String</span><span class="sxs-lookup"><span data-stu-id="29c62-124">String</span></span>|<span data-ttu-id="29c62-125">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="29c62-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="29c62-126">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="29c62-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="29c62-127">Int32</span><span class="sxs-lookup"><span data-stu-id="29c62-127">Int32</span></span>|<span data-ttu-id="29c62-128">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="29c62-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="29c62-129">Допустимые значения — от 1 до 99</span><span class="sxs-lookup"><span data-stu-id="29c62-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="29c62-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="29c62-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="29c62-131">Int32</span><span class="sxs-lookup"><span data-stu-id="29c62-131">Int32</span></span>|<span data-ttu-id="29c62-132">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="29c62-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="29c62-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="29c62-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="29c62-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="29c62-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="29c62-135">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="29c62-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="29c62-136">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="29c62-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29c62-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="29c62-137">Relationships</span></span>
<span data-ttu-id="29c62-138">Нет</span><span class="sxs-lookup"><span data-stu-id="29c62-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29c62-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29c62-139">JSON Representation</span></span>
<span data-ttu-id="29c62-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29c62-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```





