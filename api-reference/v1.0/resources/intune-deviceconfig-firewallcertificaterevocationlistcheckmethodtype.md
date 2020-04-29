---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7f2b3804878b825b0e7eed9a9ed9253abf475f1e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445959"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="2bacc-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="2bacc-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="2bacc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bacc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bacc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2bacc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bacc-106">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="2bacc-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="2bacc-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2bacc-107">Members</span></span>
|<span data-ttu-id="2bacc-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2bacc-108">Member</span></span>|<span data-ttu-id="2bacc-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2bacc-109">Value</span></span>|<span data-ttu-id="2bacc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2bacc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bacc-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="2bacc-111">deviceDefault</span></span>|<span data-ttu-id="2bacc-112">нуль</span><span class="sxs-lookup"><span data-stu-id="2bacc-112">0</span></span>|<span data-ttu-id="2bacc-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="2bacc-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="2bacc-114">Нет</span><span class="sxs-lookup"><span data-stu-id="2bacc-114">none</span></span>|<span data-ttu-id="2bacc-115">1,1</span><span class="sxs-lookup"><span data-stu-id="2bacc-115">1</span></span>|<span data-ttu-id="2bacc-116">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="2bacc-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="2bacc-117">произошл</span><span class="sxs-lookup"><span data-stu-id="2bacc-117">attempt</span></span>|<span data-ttu-id="2bacc-118">2</span><span class="sxs-lookup"><span data-stu-id="2bacc-118">2</span></span>|<span data-ttu-id="2bacc-119">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="2bacc-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="2bacc-120">необходимость</span><span class="sxs-lookup"><span data-stu-id="2bacc-120">require</span></span>|<span data-ttu-id="2bacc-121">4</span><span class="sxs-lookup"><span data-stu-id="2bacc-121">3</span></span>|<span data-ttu-id="2bacc-122">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="2bacc-122">Require a successful CRL check before allowing a certificate</span></span>|







