---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a475f32d4572b0aa8ed2a52befc7a58eb6077253
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257633"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="2e9f1-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="2e9f1-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="2e9f1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e9f1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e9f1-105">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="2e9f1-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="2e9f1-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="2e9f1-106">Members</span></span>
|<span data-ttu-id="2e9f1-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="2e9f1-107">Member</span></span>|<span data-ttu-id="2e9f1-108">Значение</span><span class="sxs-lookup"><span data-stu-id="2e9f1-108">Value</span></span>|<span data-ttu-id="2e9f1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2e9f1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e9f1-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="2e9f1-110">deviceDefault</span></span>|<span data-ttu-id="2e9f1-111">нуль</span><span class="sxs-lookup"><span data-stu-id="2e9f1-111">0</span></span>|<span data-ttu-id="2e9f1-112">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="2e9f1-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="2e9f1-113">Нет</span><span class="sxs-lookup"><span data-stu-id="2e9f1-113">none</span></span>|<span data-ttu-id="2e9f1-114">1,1</span><span class="sxs-lookup"><span data-stu-id="2e9f1-114">1</span></span>|<span data-ttu-id="2e9f1-115">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="2e9f1-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="2e9f1-116">произошл</span><span class="sxs-lookup"><span data-stu-id="2e9f1-116">attempt</span></span>|<span data-ttu-id="2e9f1-117">2</span><span class="sxs-lookup"><span data-stu-id="2e9f1-117">2</span></span>|<span data-ttu-id="2e9f1-118">Проверка списка ОТЗЫВА сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="2e9f1-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="2e9f1-119">необходимость</span><span class="sxs-lookup"><span data-stu-id="2e9f1-119">require</span></span>|<span data-ttu-id="2e9f1-120">4</span><span class="sxs-lookup"><span data-stu-id="2e9f1-120">3</span></span>|<span data-ttu-id="2e9f1-121">Требовать успешную проверку списка ОТЗЫВА сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="2e9f1-121">Require a successful CRL check before allowing a certificate</span></span>|



