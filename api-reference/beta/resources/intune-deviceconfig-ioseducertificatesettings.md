---
title: Тип ресурса Иоседуцертификатесеттингс
description: Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d9060c28744bae52d4690bf75487e298d58d2a1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800933"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="54731-103">Тип ресурса Иоседуцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="54731-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="54731-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54731-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54731-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54731-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54731-106">Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="54731-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="54731-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="54731-107">Properties</span></span>
|<span data-ttu-id="54731-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="54731-108">Property</span></span>|<span data-ttu-id="54731-109">Тип</span><span class="sxs-lookup"><span data-stu-id="54731-109">Type</span></span>|<span data-ttu-id="54731-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54731-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54731-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="54731-111">trustedRootCertificate</span></span>|<span data-ttu-id="54731-112">Binary</span><span class="sxs-lookup"><span data-stu-id="54731-112">Binary</span></span>|<span data-ttu-id="54731-113">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="54731-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="54731-114">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="54731-114">certFileName</span></span>|<span data-ttu-id="54731-115">String</span><span class="sxs-lookup"><span data-stu-id="54731-115">String</span></span>|<span data-ttu-id="54731-116">Имя файла, отображаемое в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе.</span><span class="sxs-lookup"><span data-stu-id="54731-116">File name to display in UI.</span></span>|
|<span data-ttu-id="54731-117">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="54731-117">certificationAuthority</span></span>|<span data-ttu-id="54731-118">String</span><span class="sxs-lookup"><span data-stu-id="54731-118">String</span></span>|<span data-ttu-id="54731-119">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="54731-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="54731-120">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="54731-120">certificationAuthorityName</span></span>|<span data-ttu-id="54731-121">String</span><span class="sxs-lookup"><span data-stu-id="54731-121">String</span></span>|<span data-ttu-id="54731-122">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="54731-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="54731-123">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="54731-123">certificateTemplateName</span></span>|<span data-ttu-id="54731-124">String</span><span class="sxs-lookup"><span data-stu-id="54731-124">String</span></span>|<span data-ttu-id="54731-125">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="54731-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="54731-126">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="54731-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="54731-127">Int32</span><span class="sxs-lookup"><span data-stu-id="54731-127">Int32</span></span>|<span data-ttu-id="54731-128">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="54731-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="54731-129">Допустимые значения — от 1 до 99</span><span class="sxs-lookup"><span data-stu-id="54731-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="54731-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="54731-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="54731-131">Int32</span><span class="sxs-lookup"><span data-stu-id="54731-131">Int32</span></span>|<span data-ttu-id="54731-132">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="54731-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="54731-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="54731-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="54731-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="54731-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="54731-135">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="54731-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="54731-136">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="54731-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54731-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="54731-137">Relationships</span></span>
<span data-ttu-id="54731-138">Нет</span><span class="sxs-lookup"><span data-stu-id="54731-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54731-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54731-139">JSON Representation</span></span>
<span data-ttu-id="54731-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54731-140">Here is a JSON representation of the resource.</span></span>
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





