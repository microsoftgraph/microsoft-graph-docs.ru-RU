---
title: тип списка firewallCertificateRevocationListCheckMethodType
description: Возможные значения брандмауэраCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 779cfe8b8576d475df62ed112709aa0c2e9b6c63
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754729"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="92865-103">тип списка firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="92865-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="92865-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92865-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92865-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92865-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92865-106">Возможные значения брандмауэраCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="92865-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="92865-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="92865-107">Members</span></span>
|<span data-ttu-id="92865-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="92865-108">Member</span></span>|<span data-ttu-id="92865-109">Значение</span><span class="sxs-lookup"><span data-stu-id="92865-109">Value</span></span>|<span data-ttu-id="92865-110">Описание</span><span class="sxs-lookup"><span data-stu-id="92865-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92865-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="92865-111">deviceDefault</span></span>|<span data-ttu-id="92865-112">0</span><span class="sxs-lookup"><span data-stu-id="92865-112">0</span></span>|<span data-ttu-id="92865-113">Нет значения, настроенного Intune, не переопределять настроенное пользователем значение по умолчанию устройства</span><span class="sxs-lookup"><span data-stu-id="92865-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="92865-114">нет</span><span class="sxs-lookup"><span data-stu-id="92865-114">none</span></span>|<span data-ttu-id="92865-115">1</span><span class="sxs-lookup"><span data-stu-id="92865-115">1</span></span>|<span data-ttu-id="92865-116">Не проверяйте список отзывов сертификатов</span><span class="sxs-lookup"><span data-stu-id="92865-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="92865-117">попытка</span><span class="sxs-lookup"><span data-stu-id="92865-117">attempt</span></span>|<span data-ttu-id="92865-118">2</span><span class="sxs-lookup"><span data-stu-id="92865-118">2</span></span>|<span data-ttu-id="92865-119">Попытка проверки CRL и разрешить сертификат только в том случае, если сертификат подтвержден проверкой</span><span class="sxs-lookup"><span data-stu-id="92865-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="92865-120">требовать</span><span class="sxs-lookup"><span data-stu-id="92865-120">require</span></span>|<span data-ttu-id="92865-121">3</span><span class="sxs-lookup"><span data-stu-id="92865-121">3</span></span>|<span data-ttu-id="92865-122">Требуется успешная проверка CRL перед разрешением сертификата</span><span class="sxs-lookup"><span data-stu-id="92865-122">Require a successful CRL check before allowing a certificate</span></span>|




