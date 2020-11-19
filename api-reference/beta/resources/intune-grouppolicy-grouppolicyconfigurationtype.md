---
title: тип перечисления Граупполициконфигуратионтипе
description: Тип конфигурации групповой политики
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 430fb8e88cb2f07677b9a9d9c3e959df0bedba83
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267182"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="b9737-103">тип перечисления Граупполициконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="b9737-103">groupPolicyConfigurationType enum type</span></span>

<span data-ttu-id="b9737-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9737-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9737-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9737-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9737-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9737-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9737-107">Тип конфигурации групповой политики</span><span class="sxs-lookup"><span data-stu-id="b9737-107">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="b9737-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b9737-108">Members</span></span>
|<span data-ttu-id="b9737-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b9737-109">Member</span></span>|<span data-ttu-id="b9737-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b9737-110">Value</span></span>|<span data-ttu-id="b9737-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b9737-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9737-112">policy</span><span class="sxs-lookup"><span data-stu-id="b9737-112">policy</span></span>|<span data-ttu-id="b9737-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b9737-113">0</span></span>|<span data-ttu-id="b9737-114">Тип политики не является восстановленным значением, что означает, что значение удаляется, что позволяет использовать исходное значение конфигурации.</span><span class="sxs-lookup"><span data-stu-id="b9737-114">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="b9737-115">Тип политики заменяется параметром конфигурации приложения, поэтому приложение всегда знает значение.</span><span class="sxs-lookup"><span data-stu-id="b9737-115">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="b9737-116">Тип политики не позволяет пользователю изменять значение с помощью пользовательского интерфейса приложения.</span><span class="sxs-lookup"><span data-stu-id="b9737-116">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="b9737-117">параметров</span><span class="sxs-lookup"><span data-stu-id="b9737-117">preference</span></span>|<span data-ttu-id="b9737-118">1,1</span><span class="sxs-lookup"><span data-stu-id="b9737-118">1</span></span>|<span data-ttu-id="b9737-119">Тип предпочтения приводит к восстановлению значения, которое означает, что значение не удаляется из реестра.</span><span class="sxs-lookup"><span data-stu-id="b9737-119">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="b9737-120">Тип предпочтения перезапишет настраиваемое значение пользователем и не сохранит предыдущее значение.</span><span class="sxs-lookup"><span data-stu-id="b9737-120">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="b9737-121">Тип предпочтения не запрещает пользователю изменять значение с помощью пользовательского интерфейса приложения.</span><span class="sxs-lookup"><span data-stu-id="b9737-121">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|




