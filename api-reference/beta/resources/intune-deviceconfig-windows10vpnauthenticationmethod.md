---
title: Тип перечисления windows10VpnAuthenticationMethod
description: Типы подключений к виртуальной частной сети Windows 10.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b3613436b5df458f05fefc9037b8aadbc1265385
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810971"
---
# <a name="windows10vpnauthenticationmethod-enum-type"></a><span data-ttu-id="1d7a8-103">Тип перечисления windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1d7a8-103">windows10VpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="1d7a8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d7a8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d7a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d7a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d7a8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d7a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d7a8-107">Типы подключений к виртуальной частной сети Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1d7a8-107">Windows 10 VPN connection types.</span></span>
## <a name="members"></a><span data-ttu-id="1d7a8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1d7a8-108">Members</span></span>
|<span data-ttu-id="1d7a8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1d7a8-109">Member</span></span>|<span data-ttu-id="1d7a8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1d7a8-110">Value</span></span>|<span data-ttu-id="1d7a8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1d7a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d7a8-112">certificate</span><span class="sxs-lookup"><span data-stu-id="1d7a8-112">certificate</span></span>|<span data-ttu-id="1d7a8-113">0</span><span class="sxs-lookup"><span data-stu-id="1d7a8-113">0</span></span>|<span data-ttu-id="1d7a8-114">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="1d7a8-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="1d7a8-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="1d7a8-115">usernameAndPassword</span></span>|<span data-ttu-id="1d7a8-116">1</span><span class="sxs-lookup"><span data-stu-id="1d7a8-116">1</span></span>|<span data-ttu-id="1d7a8-117">Использовать имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="1d7a8-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="1d7a8-118">customEapXml</span><span class="sxs-lookup"><span data-stu-id="1d7a8-118">customEapXml</span></span>|<span data-ttu-id="1d7a8-119">2</span><span class="sxs-lookup"><span data-stu-id="1d7a8-119">2</span></span>|<span data-ttu-id="1d7a8-120">Метод проверки подлинности указан в XML настраиваемого поставщика внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="1d7a8-120">Authentication method is specified in custom EAP XML.</span></span>|





