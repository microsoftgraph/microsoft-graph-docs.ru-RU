---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ad3ff24cc902a943fd9c146310d58cd1f1bfbd8d
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088121"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="b2c06-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="b2c06-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="b2c06-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2c06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2c06-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2c06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2c06-106">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="b2c06-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="b2c06-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b2c06-107">Members</span></span>
|<span data-ttu-id="b2c06-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b2c06-108">Member</span></span>|<span data-ttu-id="b2c06-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b2c06-109">Value</span></span>|<span data-ttu-id="b2c06-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b2c06-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2c06-111">certificate</span><span class="sxs-lookup"><span data-stu-id="b2c06-111">certificate</span></span>|<span data-ttu-id="b2c06-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b2c06-112">0</span></span>|<span data-ttu-id="b2c06-113">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="b2c06-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="b2c06-114">усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="b2c06-114">usernameAndPassword</span></span>|<span data-ttu-id="b2c06-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b2c06-115">1</span></span>|<span data-ttu-id="b2c06-116">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b2c06-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="b2c06-117">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="b2c06-117">sharedSecret</span></span>|<span data-ttu-id="b2c06-118">2</span><span class="sxs-lookup"><span data-stu-id="b2c06-118">2</span></span>|<span data-ttu-id="b2c06-119">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b2c06-119">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="b2c06-120">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="b2c06-120">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="b2c06-121">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="b2c06-121">derivedCredential</span></span>|<span data-ttu-id="b2c06-122">4</span><span class="sxs-lookup"><span data-stu-id="b2c06-122">3</span></span>|<span data-ttu-id="b2c06-123">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b2c06-123">Use Derived Credential for Authentication.</span></span>|



