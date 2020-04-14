---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f220d5e592544ec3527c16c425d4b22fe0266d4c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444311"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="7a496-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="7a496-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="7a496-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a496-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a496-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a496-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a496-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a496-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a496-107">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="7a496-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="7a496-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7a496-108">Members</span></span>
|<span data-ttu-id="7a496-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7a496-109">Member</span></span>|<span data-ttu-id="7a496-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7a496-110">Value</span></span>|<span data-ttu-id="7a496-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7a496-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a496-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="7a496-112">deviceDefault</span></span>|<span data-ttu-id="7a496-113">нуль</span><span class="sxs-lookup"><span data-stu-id="7a496-113">0</span></span>|<span data-ttu-id="7a496-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="7a496-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="7a496-115">нет</span><span class="sxs-lookup"><span data-stu-id="7a496-115">none</span></span>|<span data-ttu-id="7a496-116">1,1</span><span class="sxs-lookup"><span data-stu-id="7a496-116">1</span></span>|<span data-ttu-id="7a496-117">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="7a496-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="7a496-118">произошл</span><span class="sxs-lookup"><span data-stu-id="7a496-118">attempt</span></span>|<span data-ttu-id="7a496-119">2</span><span class="sxs-lookup"><span data-stu-id="7a496-119">2</span></span>|<span data-ttu-id="7a496-120">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="7a496-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="7a496-121">необходимость</span><span class="sxs-lookup"><span data-stu-id="7a496-121">require</span></span>|<span data-ttu-id="7a496-122">4</span><span class="sxs-lookup"><span data-stu-id="7a496-122">3</span></span>|<span data-ttu-id="7a496-123">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="7a496-123">Require a successful CRL check before allowing a certificate</span></span>|



