---
title: Развертывание, тестирование и расширение перенесенных приложений
description: 'Описывает миграцию приложений Azure Active Directory (Azure AD) для использования API Microsoft Graph (REST); в этом рассмотрен шаг 3: развертывание, тестирование и расширение.'
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 6460b768381cdf3223699d95d1d5b9ce9ed629e8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761292"
---
# <a name="deploy-test-and-extend"></a>Развертывание, тестирование и расширение

Это шаг 4 процесса [миграции приложений.](migrate-azure-ad-graph-planning-checklist.md)

1.  **Полностью протестировать**

    После обновления приложения тщательно проверьте его, чтобы убедиться, что оно работает как ожидалось, и что вы не представили никаких регрессий.  

    Не забудьте использовать несколько сред, наборов данных и лиц конечного пользователя, например учетные данные с различными ролями, правами и обязанностями. Пройдите весь жизненный цикл, впервые получив нового тестового пользователя, а также существующего пользователя (который уже дал согласие) на повторное использование приложения.

2.  **Развертывание поэтапного обновления**

    Рассмотрите возможность развертывания обновлений поэтапно.  Ограниченный доступ к небольшому набору дружественных пользователей может помочь выявить сбои и другие потенциально неуловимые проблемы.  Это также позволяет отслеживать начальный прием и обратную связь.

    Если первоначальный развертывание проходит хорошо, отслеживайте ход развертывания в более крупных аудиториях.

3.  **Изучение нового значения**

    Теперь, когда вы перешли на Microsoft Graph, вам никогда не было проще разблокировать множество наборов данных и функций, которые теперь находятся у вас под рукой. 
    Microsoft Graph поддерживает множество новых наборов данных и функций Azure AD, недоступных в Azure AD Graph, в том числе: 

    - [Управление группой Microsoft 365](./office365-groups-concept-overview.md)
    - [Внешние приглашения пользователей](/graph/api/resources/invitation?view=graph-rest-1.0)
    - Возможность восстановления [пользователей и групп Microsoft 365](/graph/api/resources/directory?view=graph-rest-1.0) после удаления
    - [Уведомления webhook для пользователей и групп](./webhooks.md?toc=.%252fref%252ftoc.json&view=graph-rest-1.0)
    - Функции управления удостоверением, такие как:
      - [Привилегированное управление удостоверениями](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) для повышения пользователей до привилегированных ролей только при необходимости и в течение ограниченного периода времени
      - [Обзоры](/graph/api/resources/accessreviews-root?view=graph-rest-beta) доступа для одновентных или повторяющихся обзоров доступа для проверки прав доступа пользователя
      - [Условия использования, позволяющие](/graph/api/resources/accessreviews-root?view=graph-rest-beta) организациям представлять информацию для юридических или нормативных требований, например уведомлений об отказе от ответственности.
    - Функции безопасности, такие как:
      - [События с риском для идентификации](/graph/api/resources/identityriskevent?view=graph-rest-1.0)
      - [Рискованные пользователи](/graph/api/resources/riskyuser?view=graph-rest-1.0)
    - [Клиентские библиотеки и примеры,](./index.yml) доступные на многих других платформах и языках. SDKs Microsoft Graph предоставляют обнаруживаемый интерфейс для легкого доступа к данным при прозрачной обработке приобретения маркеров, обработки повторной обработки из-за ошибок и регулирования, безопасной обработки перенаправления и сериализации моделей и десериализации.

    Microsoft Graph предоставляет доступ к гораздо большему набору служб, чем только Azure Active Directory. Это шлюз [API для служб Microsoft 365 тоже](./index.yml).
    Регулярно проверяйте новые наборы данных и возможности.  

    - Посмотрите, что [можно сделать с Microsoft Graph](/graph/examples)
    - Ознакомьтесь [с последними новостями](/graph/blogs) о Microsoft Graph и некоторыми отличными сериями обучения в блоге Microsoft Graph.
    - В [статье changelog](/greaph/changelog) обобщаются обновления службы и документов. После этих обновлений вы сможете отслеживать новые API, введенные в /бета-версию (предварительный просмотр), и те, которые повышены до v1.0 (GA).  Эти новые API могут предоставить новые возможности для добавления дополнительных значений и новых функций в приложения.  

## <a name="see-also"></a>См. также

Если в процессе миграции возникают проблемы или требуется помощь, вы можете:

- Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список
- Публикация вопросов [в Microsoft Q&A](https://docs.microsoft.com/answers/topics/microsoft-graph-applications.html) 
- Просмотрите примеры Microsoft Graph, чтобы сравнить их с существующим кодом приложения:
  - **Приложения, которые используют API REST:** изучить быстрые запуски и [примеры,](https://developer.microsoft.com/graph/get-started)выбрав платформу выбора и выполнить быстрый запуск или поиск соответствующего примера
  - **Приложение, которое использует клиентскую** библиотеку .NET: обзор [консоли-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) and/or [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)

## <a name="next-steps"></a>Дальнейшие действия

- Используйте [быстрые старты и примеры,](/graph/get-started) чтобы быстро ускориться.
- Использование [клиентских библиотек и SDKs для](https://developer.microsoft.com/graph/get-started) разработки настраиваемого приложения 
- Ознакомьтесь с концепциями и практиками [Microsoft Graph.](./overview.md)
- Используйте [Graph Explorer](https://aka.ms/ge) для экспериментов с Microsoft Graph.