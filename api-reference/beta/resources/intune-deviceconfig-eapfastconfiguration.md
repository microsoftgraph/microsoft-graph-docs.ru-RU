---
title: тип перечисления Еапфастконфигуратион
description: Доступные параметры настройки EAP – FAST.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1dbb99ef309f1fe3bb85030ba681552da3548f06
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280636"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="e052c-103">тип перечисления Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e052c-103">eapFastConfiguration enum type</span></span>

<span data-ttu-id="e052c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e052c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e052c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e052c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e052c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e052c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e052c-107">Доступные параметры настройки EAP – FAST.</span><span class="sxs-lookup"><span data-stu-id="e052c-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="e052c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e052c-108">Members</span></span>
|<span data-ttu-id="e052c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e052c-109">Member</span></span>|<span data-ttu-id="e052c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e052c-110">Value</span></span>|<span data-ttu-id="e052c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e052c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e052c-112">нопротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="e052c-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="e052c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="e052c-113">0</span></span>|<span data-ttu-id="e052c-114">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="e052c-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="e052c-115">усепротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="e052c-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="e052c-116">1,1</span><span class="sxs-lookup"><span data-stu-id="e052c-116">1</span></span>|<span data-ttu-id="e052c-117">Использование учетных данных безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="e052c-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="e052c-118">усепротектедакцесскредентиаландпровисион</span><span class="sxs-lookup"><span data-stu-id="e052c-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="e052c-119">2</span><span class="sxs-lookup"><span data-stu-id="e052c-119">2</span></span>|<span data-ttu-id="e052c-120">Использование учетных данных безопасного доступа (PAC) и подготовка ключа PAC.</span><span class="sxs-lookup"><span data-stu-id="e052c-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="e052c-121">усепротектедакцесскредентиаландпровисионанонимаусли</span><span class="sxs-lookup"><span data-stu-id="e052c-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="e052c-122">4</span><span class="sxs-lookup"><span data-stu-id="e052c-122">3</span></span>|<span data-ttu-id="e052c-123">Использование учетных данных безопасного доступа (PAC), подготовка ключа PAC и анонимное выполнение.</span><span class="sxs-lookup"><span data-stu-id="e052c-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|




