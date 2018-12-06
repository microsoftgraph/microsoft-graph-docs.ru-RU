---
title: Поток данных API безопасности Microsoft Graph
description: API безопасности Microsoft Graph объединяет в федерацию запросы ко всем поставщикам услуг в экосистеме безопасности Microsoft Graph. Она основана на согласии поставщика услуг безопасности, предоставляемом приложением, как показано на схеме ниже. Рабочий процесс получения согласия относится только к сторонним поставщикам услуг.
ms.openlocfilehash: 1e8b074e3cf4589ca67364ed7e225a62f40300fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092661"
---
# <a name="microsoft-graph-security-api-data-flow"></a><span data-ttu-id="c082f-105">Поток данных API безопасности Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c082f-105">Microsoft Graph Security API data flow</span></span>

<span data-ttu-id="c082f-106">API безопасности Microsoft Graph объединяет в федерацию запросы ко всем поставщикам услуг в экосистеме безопасности Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c082f-106">The Microsoft Graph Security API federates requests to all providers in the Microsoft Graph Security ecosystem.</span></span> <span data-ttu-id="c082f-107">Она основана на согласии поставщика услуг безопасности, предоставляемом приложением, как показано на схеме ниже.</span><span class="sxs-lookup"><span data-stu-id="c082f-107">This is based on the security provider consent provided by the application, as shown in the following diagram.</span></span> <span data-ttu-id="c082f-108">Рабочий процесс получения согласия относится только к сторонним поставщикам услуг.</span><span class="sxs-lookup"><span data-stu-id="c082f-108">The consent workflow only applies to non-Microsoft providers.</span></span>

![security_dataflow_1.png](./images/security-dataflow-1.png)

<span data-ttu-id="c082f-110">Ниже приведено описание потока:</span><span class="sxs-lookup"><span data-stu-id="c082f-110">The following is a description of the flow:</span></span>

1. <span data-ttu-id="c082f-111">Пользователь входит в приложение поставщика для просмотра формы согласия поставщика услуг.</span><span class="sxs-lookup"><span data-stu-id="c082f-111">The application user signs in to the provider application to view the consent form from the provider.</span></span> <span data-ttu-id="c082f-112">Эта интерфейс, в котором отображается форма согласия, принадлежит поставщику и относится к сторонним поставщикам. Форма требуется только для получения явного согласия клиентов на отправку запросов к API безопасности Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c082f-112">This consent form experience or UI is owned by the provider and applies to non-Microsoft providers only to get explicit consent from their customers to send requests to Microsoft Graph Security API.</span></span>
2. <span data-ttu-id="c082f-113">Согласие клиента хранится у поставщика услуг.</span><span class="sxs-lookup"><span data-stu-id="c082f-113">The client consent is stored on the provider side.</span></span>
3. <span data-ttu-id="c082f-114">Служба согласия поставщика услуг вызывает API безопасности Microsoft Graph, чтобы утвердить согласие соответствующего клиента.</span><span class="sxs-lookup"><span data-stu-id="c082f-114">The provider consent service calls the Microsoft Graph Security API to inform consent approval for the respective customer.</span></span>
4. <span data-ttu-id="c082f-115">Приложение отправляет запрос в API безопасности Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c082f-115">The application sends a request to the Microsoft Graph Security API.</span></span>
5. <span data-ttu-id="c082f-116">API безопасности Microsoft Graph проверяет сведения разрешения для этого клиента, сопоставляя их с различными поставщиками услуг.</span><span class="sxs-lookup"><span data-stu-id="c082f-116">The Microsoft Graph Security API checks for the consent information for this customer mapped to various providers.</span></span>
6. <span data-ttu-id="c082f-117">API безопасности Microsoft Graph вызывает всех поставщиков услуг, которым клиент предоставил явное согласие с помощью их специальных форм.</span><span class="sxs-lookup"><span data-stu-id="c082f-117">The Microsoft Graph Security API calls all those providers the customer has given explicit consent to via the provider consent experience.</span></span>
7. <span data-ttu-id="c082f-118">Возвращается ответ от всех поставщиков, которые получили согласие этого клиента.</span><span class="sxs-lookup"><span data-stu-id="c082f-118">The response is returned from all the consented providers for that client.</span></span>
8. <span data-ttu-id="c082f-119">Ответ в виде набора результатов возвращается в приложение.</span><span class="sxs-lookup"><span data-stu-id="c082f-119">The result set response is returned to the application.</span></span>
9. <span data-ttu-id="c082f-120">Если клиент не давал согласия ни одному поставщику услуг, их результаты не включаются в ответ.</span><span class="sxs-lookup"><span data-stu-id="c082f-120">If the customer has not consented to any provider, no results from those providers are included in the response.</span></span>
