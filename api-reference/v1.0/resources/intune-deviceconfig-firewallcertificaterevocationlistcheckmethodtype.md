---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7c5fa3baaeb3d24bc902d733a6c6462fbcf70f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028303"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="1b735-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="1b735-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="1b735-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b735-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b735-105">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="1b735-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="1b735-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="1b735-106">Members</span></span>
|<span data-ttu-id="1b735-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="1b735-107">Member</span></span>|<span data-ttu-id="1b735-108">Значение</span><span class="sxs-lookup"><span data-stu-id="1b735-108">Value</span></span>|<span data-ttu-id="1b735-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1b735-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b735-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="1b735-110">deviceDefault</span></span>|<span data-ttu-id="1b735-111">нуль</span><span class="sxs-lookup"><span data-stu-id="1b735-111">0</span></span>|<span data-ttu-id="1b735-112">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="1b735-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="1b735-113">none</span><span class="sxs-lookup"><span data-stu-id="1b735-113">none</span></span>|<span data-ttu-id="1b735-114">1,1</span><span class="sxs-lookup"><span data-stu-id="1b735-114">1</span></span>|<span data-ttu-id="1b735-115">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="1b735-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="1b735-116">произошл</span><span class="sxs-lookup"><span data-stu-id="1b735-116">attempt</span></span>|<span data-ttu-id="1b735-117">2</span><span class="sxs-lookup"><span data-stu-id="1b735-117">2</span></span>|<span data-ttu-id="1b735-118">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="1b735-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="1b735-119">необходимость</span><span class="sxs-lookup"><span data-stu-id="1b735-119">require</span></span>|<span data-ttu-id="1b735-120">4</span><span class="sxs-lookup"><span data-stu-id="1b735-120">3</span></span>|<span data-ttu-id="1b735-121">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="1b735-121">Require a successful CRL check before allowing a certificate</span></span>|



