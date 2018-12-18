---
title: Тип перечисления firewallCertificateRevocationListCheckMethodType
description: Возможные значения для firewallCertificateRevocationListCheckMethod
author: tfitzmac
ms.openlocfilehash: 302037187addfb8606c6c1e60a9369eb1f7c2ed5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320715"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="f2baa-103">Тип перечисления firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="f2baa-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="f2baa-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2baa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2baa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2baa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2baa-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f2baa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2baa-107">Возможные значения для firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="f2baa-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="f2baa-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f2baa-108">Members</span></span>
|<span data-ttu-id="f2baa-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f2baa-109">Member</span></span>|<span data-ttu-id="f2baa-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f2baa-110">Value</span></span>|<span data-ttu-id="f2baa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f2baa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2baa-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f2baa-112">deviceDefault</span></span>|<span data-ttu-id="f2baa-113">0</span><span class="sxs-lookup"><span data-stu-id="f2baa-113">0</span></span>|<span data-ttu-id="f2baa-114">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="f2baa-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="f2baa-115">none</span><span class="sxs-lookup"><span data-stu-id="f2baa-115">none</span></span>|<span data-ttu-id="f2baa-116">1</span><span class="sxs-lookup"><span data-stu-id="f2baa-116">1</span></span>|<span data-ttu-id="f2baa-117">Не проверять списка отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="f2baa-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="f2baa-118">Попытка</span><span class="sxs-lookup"><span data-stu-id="f2baa-118">attempt</span></span>|<span data-ttu-id="f2baa-119">2</span><span class="sxs-lookup"><span data-stu-id="f2baa-119">2</span></span>|<span data-ttu-id="f2baa-120">Попытайтесь проверки списка отзыва Сертификатов и разрешить сертификат только в том случае, если сертификат подтверждается при проверке</span><span class="sxs-lookup"><span data-stu-id="f2baa-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="f2baa-121">Требовать</span><span class="sxs-lookup"><span data-stu-id="f2baa-121">require</span></span>|<span data-ttu-id="f2baa-122">3</span><span class="sxs-lookup"><span data-stu-id="f2baa-122">3</span></span>|<span data-ttu-id="f2baa-123">Требовать успешной проверки списка отзыва Сертификатов, перед тем как разрешить сертификата</span><span class="sxs-lookup"><span data-stu-id="f2baa-123">Require a successful CRL check before allowing a certificate</span></span>|





