---
title: тип перечисления Емаилцертификатетипе
description: Поддерживаемые источники сертификатов для подписи и шифрования электронной почты.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 266bc9e0b23009f34281c70095176ccd88b50907
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526474"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="4845b-103">тип перечисления Емаилцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="4845b-103">emailCertificateType enum type</span></span>

<span data-ttu-id="4845b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4845b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4845b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4845b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4845b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4845b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4845b-107">Поддерживаемые источники сертификатов для подписи и шифрования электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4845b-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="4845b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4845b-108">Members</span></span>
|<span data-ttu-id="4845b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4845b-109">Member</span></span>|<span data-ttu-id="4845b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4845b-110">Value</span></span>|<span data-ttu-id="4845b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4845b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4845b-112">нет</span><span class="sxs-lookup"><span data-stu-id="4845b-112">none</span></span>|<span data-ttu-id="4845b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="4845b-113">0</span></span>|<span data-ttu-id="4845b-114">Не используйте сертификат в качестве источника.</span><span class="sxs-lookup"><span data-stu-id="4845b-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="4845b-115">certificate</span><span class="sxs-lookup"><span data-stu-id="4845b-115">certificate</span></span>|<span data-ttu-id="4845b-116">1 </span><span class="sxs-lookup"><span data-stu-id="4845b-116">1</span></span>|<span data-ttu-id="4845b-117">Используйте сертификат для источника сертификата.</span><span class="sxs-lookup"><span data-stu-id="4845b-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="4845b-118">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="4845b-118">derivedCredential</span></span>|<span data-ttu-id="4845b-119">2 </span><span class="sxs-lookup"><span data-stu-id="4845b-119">2</span></span>|<span data-ttu-id="4845b-120">Использование производных учетных данных для источника сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4845b-120">Use a derived credential for certificate source.</span></span>|



