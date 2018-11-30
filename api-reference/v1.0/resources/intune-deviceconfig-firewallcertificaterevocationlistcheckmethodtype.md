---
title: Тип перечисления firewallCertificateRevocationListCheckMethodType
description: Возможные значения для firewallCertificateRevocationListCheckMethod
ms.openlocfilehash: b6a7d702b1156598387c204d9e42b15f3066598d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027146"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="1ca05-103">Тип перечисления firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="1ca05-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="1ca05-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1ca05-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ca05-105">Возможные значения для firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="1ca05-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="1ca05-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="1ca05-106">Members</span></span>
|<span data-ttu-id="1ca05-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="1ca05-107">Member</span></span>|<span data-ttu-id="1ca05-108">Значение</span><span class="sxs-lookup"><span data-stu-id="1ca05-108">Value</span></span>|<span data-ttu-id="1ca05-109">Description</span><span class="sxs-lookup"><span data-stu-id="1ca05-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ca05-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1ca05-110">deviceDefault</span></span>|<span data-ttu-id="1ca05-111">0</span><span class="sxs-lookup"><span data-stu-id="1ca05-111">0</span></span>|<span data-ttu-id="1ca05-112">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="1ca05-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="1ca05-113">Нет</span><span class="sxs-lookup"><span data-stu-id="1ca05-113">none</span></span>|<span data-ttu-id="1ca05-114">1</span><span class="sxs-lookup"><span data-stu-id="1ca05-114">1</span></span>|<span data-ttu-id="1ca05-115">Не проверять списка отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="1ca05-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="1ca05-116">Попытка</span><span class="sxs-lookup"><span data-stu-id="1ca05-116">attempt</span></span>|<span data-ttu-id="1ca05-117">2</span><span class="sxs-lookup"><span data-stu-id="1ca05-117">2</span></span>|<span data-ttu-id="1ca05-118">Попытайтесь проверки списка отзыва Сертификатов и разрешить сертификат только в том случае, если сертификат подтверждается при проверке</span><span class="sxs-lookup"><span data-stu-id="1ca05-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="1ca05-119">Требовать</span><span class="sxs-lookup"><span data-stu-id="1ca05-119">require</span></span>|<span data-ttu-id="1ca05-120">3</span><span class="sxs-lookup"><span data-stu-id="1ca05-120">3</span></span>|<span data-ttu-id="1ca05-121">Требовать успешной проверки списка отзыва Сертификатов, перед тем как разрешить сертификата</span><span class="sxs-lookup"><span data-stu-id="1ca05-121">Require a successful CRL check before allowing a certificate</span></span>|



