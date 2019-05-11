---
title: тип перечисления Емаилцертификатетипе
description: Поддерживаемые источники сертификатов для подписи и шифрования электронной почты.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 150109f68d4cac95c07d2bc973149b1309fefc07
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33957102"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="76917-103">тип перечисления Емаилцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="76917-103">emailCertificateType enum type</span></span>

> <span data-ttu-id="76917-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76917-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76917-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76917-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76917-106">Поддерживаемые источники сертификатов для подписи и шифрования электронной почты.</span><span class="sxs-lookup"><span data-stu-id="76917-106">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="76917-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="76917-107">Members</span></span>
|<span data-ttu-id="76917-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="76917-108">Member</span></span>|<span data-ttu-id="76917-109">Значение</span><span class="sxs-lookup"><span data-stu-id="76917-109">Value</span></span>|<span data-ttu-id="76917-110">Описание</span><span class="sxs-lookup"><span data-stu-id="76917-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76917-111">none</span><span class="sxs-lookup"><span data-stu-id="76917-111">none</span></span>|<span data-ttu-id="76917-112">нуль</span><span class="sxs-lookup"><span data-stu-id="76917-112">0</span></span>|<span data-ttu-id="76917-113">Не используйте сертификат в качестве источника.</span><span class="sxs-lookup"><span data-stu-id="76917-113">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="76917-114">certificate</span><span class="sxs-lookup"><span data-stu-id="76917-114">certificate</span></span>|<span data-ttu-id="76917-115">1,1</span><span class="sxs-lookup"><span data-stu-id="76917-115">1</span></span>|<span data-ttu-id="76917-116">Используйте сертификат для источника сертификата.</span><span class="sxs-lookup"><span data-stu-id="76917-116">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="76917-117">Дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="76917-117">derivedCredential</span></span>|<span data-ttu-id="76917-118">2</span><span class="sxs-lookup"><span data-stu-id="76917-118">2</span></span>|<span data-ttu-id="76917-119">Использование производных учетных данных для источника сертификатов.</span><span class="sxs-lookup"><span data-stu-id="76917-119">Use a derived credential for certificate source.</span></span>|




