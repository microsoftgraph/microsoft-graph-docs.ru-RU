---
title: тип перечисления Еапфастконфигуратион
description: Доступные параметры настройки EAP – FAST.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8deeae69bb4d828cc2e0178c79aba200f8a4709e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946814"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="dbe23-103">тип перечисления Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="dbe23-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="dbe23-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbe23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbe23-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbe23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbe23-106">Доступные параметры настройки EAP – FAST.</span><span class="sxs-lookup"><span data-stu-id="dbe23-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="dbe23-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="dbe23-107">Members</span></span>
|<span data-ttu-id="dbe23-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="dbe23-108">Member</span></span>|<span data-ttu-id="dbe23-109">Значение</span><span class="sxs-lookup"><span data-stu-id="dbe23-109">Value</span></span>|<span data-ttu-id="dbe23-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dbe23-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbe23-111">Нопротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="dbe23-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="dbe23-112">нуль</span><span class="sxs-lookup"><span data-stu-id="dbe23-112">0</span></span>|<span data-ttu-id="dbe23-113">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="dbe23-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="dbe23-114">Усепротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="dbe23-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="dbe23-115">1,1</span><span class="sxs-lookup"><span data-stu-id="dbe23-115">1</span></span>|<span data-ttu-id="dbe23-116">Использование учетных данных безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="dbe23-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="dbe23-117">Усепротектедакцесскредентиаландпровисион</span><span class="sxs-lookup"><span data-stu-id="dbe23-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="dbe23-118">2</span><span class="sxs-lookup"><span data-stu-id="dbe23-118">2</span></span>|<span data-ttu-id="dbe23-119">Использование учетных данных безопасного доступа (PAC) и подготовка ключа PAC.</span><span class="sxs-lookup"><span data-stu-id="dbe23-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="dbe23-120">Усепротектедакцесскредентиаландпровисионанонимаусли</span><span class="sxs-lookup"><span data-stu-id="dbe23-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="dbe23-121">4</span><span class="sxs-lookup"><span data-stu-id="dbe23-121">3</span></span>|<span data-ttu-id="dbe23-122">Использование учетных данных безопасного доступа (PAC), подготовка ключа PAC и анонимное выполнение.</span><span class="sxs-lookup"><span data-stu-id="dbe23-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|




