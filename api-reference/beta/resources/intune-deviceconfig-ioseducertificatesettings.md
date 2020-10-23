---
title: Тип ресурса Иоседуцертификатесеттингс
description: Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2693075e10fc52536f130128dbadfb5d3f06c8ad
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726481"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="3842a-103">Тип ресурса Иоседуцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="3842a-103">iosEduCertificateSettings resource type</span></span>

<span data-ttu-id="3842a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3842a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3842a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3842a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3842a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3842a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3842a-107">Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="3842a-107">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="3842a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3842a-108">Properties</span></span>
|<span data-ttu-id="3842a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3842a-109">Property</span></span>|<span data-ttu-id="3842a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3842a-110">Type</span></span>|<span data-ttu-id="3842a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3842a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3842a-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="3842a-112">trustedRootCertificate</span></span>|<span data-ttu-id="3842a-113">Binary</span><span class="sxs-lookup"><span data-stu-id="3842a-113">Binary</span></span>|<span data-ttu-id="3842a-114">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="3842a-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="3842a-115">цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="3842a-115">certFileName</span></span>|<span data-ttu-id="3842a-116">Строка</span><span class="sxs-lookup"><span data-stu-id="3842a-116">String</span></span>|<span data-ttu-id="3842a-117">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="3842a-117">File name to display in UI.</span></span>|
|<span data-ttu-id="3842a-118">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="3842a-118">certificationAuthority</span></span>|<span data-ttu-id="3842a-119">Строка</span><span class="sxs-lookup"><span data-stu-id="3842a-119">String</span></span>|<span data-ttu-id="3842a-120">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="3842a-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="3842a-121">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="3842a-121">certificationAuthorityName</span></span>|<span data-ttu-id="3842a-122">Строка</span><span class="sxs-lookup"><span data-stu-id="3842a-122">String</span></span>|<span data-ttu-id="3842a-123">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="3842a-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="3842a-124">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="3842a-124">certificateTemplateName</span></span>|<span data-ttu-id="3842a-125">Строка</span><span class="sxs-lookup"><span data-stu-id="3842a-125">String</span></span>|<span data-ttu-id="3842a-126">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="3842a-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="3842a-127">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="3842a-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="3842a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="3842a-128">Int32</span></span>|<span data-ttu-id="3842a-129">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="3842a-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3842a-130">Допустимые значения — от 1 до 99</span><span class="sxs-lookup"><span data-stu-id="3842a-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="3842a-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3842a-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3842a-132">Int32</span><span class="sxs-lookup"><span data-stu-id="3842a-132">Int32</span></span>|<span data-ttu-id="3842a-133">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="3842a-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="3842a-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3842a-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3842a-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3842a-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3842a-136">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="3842a-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="3842a-137">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3842a-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3842a-138">Связи</span><span class="sxs-lookup"><span data-stu-id="3842a-138">Relationships</span></span>
<span data-ttu-id="3842a-139">Нет</span><span class="sxs-lookup"><span data-stu-id="3842a-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3842a-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3842a-140">JSON Representation</span></span>
<span data-ttu-id="3842a-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3842a-141">Here is a JSON representation of the resource.</span></span>
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





