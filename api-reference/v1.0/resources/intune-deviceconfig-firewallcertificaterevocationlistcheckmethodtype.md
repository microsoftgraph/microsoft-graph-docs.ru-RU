---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 969a94ed8a782989aaf9d34c00fe1f4cc82775ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056711"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="54003-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="54003-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="54003-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54003-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54003-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54003-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54003-106">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="54003-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="54003-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="54003-107">Members</span></span>
|<span data-ttu-id="54003-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="54003-108">Member</span></span>|<span data-ttu-id="54003-109">Значение</span><span class="sxs-lookup"><span data-stu-id="54003-109">Value</span></span>|<span data-ttu-id="54003-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54003-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54003-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="54003-111">deviceDefault</span></span>|<span data-ttu-id="54003-112">нуль</span><span class="sxs-lookup"><span data-stu-id="54003-112">0</span></span>|<span data-ttu-id="54003-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="54003-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="54003-114">Нет</span><span class="sxs-lookup"><span data-stu-id="54003-114">none</span></span>|<span data-ttu-id="54003-115">1 </span><span class="sxs-lookup"><span data-stu-id="54003-115">1</span></span>|<span data-ttu-id="54003-116">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="54003-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="54003-117">произошл</span><span class="sxs-lookup"><span data-stu-id="54003-117">attempt</span></span>|<span data-ttu-id="54003-118">2 </span><span class="sxs-lookup"><span data-stu-id="54003-118">2</span></span>|<span data-ttu-id="54003-119">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="54003-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="54003-120">необходимость</span><span class="sxs-lookup"><span data-stu-id="54003-120">require</span></span>|<span data-ttu-id="54003-121">4</span><span class="sxs-lookup"><span data-stu-id="54003-121">3</span></span>|<span data-ttu-id="54003-122">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="54003-122">Require a successful CRL check before allowing a certificate</span></span>|









