---
title: Тип перечисления windows10VpnAuthenticationMethod
description: Типы подключений к виртуальной частной сети Windows 10.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d6159a20c6fc3ad47f3ffc6f78cd3b76e1de1371
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914628"
---
# <a name="windows10vpnauthenticationmethod-enum-type"></a><span data-ttu-id="a51ef-103">Тип перечисления windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a51ef-103">windows10VpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="a51ef-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a51ef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a51ef-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a51ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a51ef-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a51ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a51ef-107">Типы подключений к виртуальной частной сети Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a51ef-107">Windows 10 VPN connection types.</span></span>
## <a name="members"></a><span data-ttu-id="a51ef-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a51ef-108">Members</span></span>
|<span data-ttu-id="a51ef-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a51ef-109">Member</span></span>|<span data-ttu-id="a51ef-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a51ef-110">Value</span></span>|<span data-ttu-id="a51ef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a51ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a51ef-112">certificate</span><span class="sxs-lookup"><span data-stu-id="a51ef-112">certificate</span></span>|<span data-ttu-id="a51ef-113">0</span><span class="sxs-lookup"><span data-stu-id="a51ef-113">0</span></span>|<span data-ttu-id="a51ef-114">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="a51ef-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="a51ef-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="a51ef-115">usernameAndPassword</span></span>|<span data-ttu-id="a51ef-116">1</span><span class="sxs-lookup"><span data-stu-id="a51ef-116">1</span></span>|<span data-ttu-id="a51ef-117">Использовать имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a51ef-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="a51ef-118">customEapXml</span><span class="sxs-lookup"><span data-stu-id="a51ef-118">customEapXml</span></span>|<span data-ttu-id="a51ef-119">2</span><span class="sxs-lookup"><span data-stu-id="a51ef-119">2</span></span>|<span data-ttu-id="a51ef-120">Метод проверки подлинности указан в XML настраиваемого поставщика внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="a51ef-120">Authentication method is specified in custom EAP XML.</span></span>|





