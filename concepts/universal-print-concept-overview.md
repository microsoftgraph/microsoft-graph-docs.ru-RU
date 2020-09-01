---
title: Обзор API облачной среды универсальной печати
description: Универсальная печать — это современное решение печати, которое можно использовать в организациях для управления инфраструктурой печати через облачные службы от Майкрософт.
author: braedenp-msft
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: b15da734583200891cc451b332cccd24a6ef47f8
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319528"
---
# <a name="universal-print-cloud-printing-api-overview"></a>Обзор API облачной среды универсальной печати

Универсальная печать — это современное решение печати, которое можно использовать в организациях для управления инфраструктурой печати через облачные службы от Майкрософт.

![Снимок экрана с изображением главной страницы универсальной печати на портале Azure](images/universal-print-portal-homepage.png)

## <a name="why-use-universal-print"></a>Зачем нужна универсальная печать?

Универсальная печать — это функции печати Windows Server, перенесенные в облако Microsoft 365, благодаря которым организации теперь могут обойтись без локальных серверов печати и не устанавливать драйверы печати на устройствах. Кроме того, в рамках универсальной печати предусмотрены дополнительные функции, например, группы безопасности для доступа к принтеру, обнаружение принтеров на основе расположения и расширенными возможностями для администраторов.

По мере внедрения универсальной печати в организациях организации и независимые поставщики программного обеспечения могут использовать API универсальной печати в Microsoft Graph, чтобы создавать и расширять приложения для поддержки новых сценариев.

### <a name="print-documents-from-web-and-mobile-applications"></a>Печать документов из веб-приложений и мобильных приложений

Благодаря перемещению инфраструктуры печати в облако печатать документы можно непосредственно из веб-приложений и мобильных приложений.

Чтобы приступить к работе с API универсальной печати, выполните указанные ниже действия.

1. [Создайте задание печати](/graph/api/printer-post-jobs?view=graph-rest-beta) и сохраните идентификатор полученного документа.
2. [Отправьте данные документа](/graph/api/printdocument-uploaddata?view=graph-rest-beta) в документ.
3. [Запустите задание печати](/graph/api/printjob-startprintjob?view=graph-rest-beta).

### <a name="manage-printers"></a>Управление принтерами

Отследить принтеры организации, настройки принтеров и их использование — непростая задача. Благодаря API универсальной печати можно интегрировать эти три направления.

* **Отслеживать состояние принтеров, их настройки и доступность**можно через [Список принтеров](/graph/api/print-list-printers?view=graph-rest-beta) и [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta).

* **Узнать, кто из пользователей использует принтеры и сколько страниц они печатают** можно через отчетные API:
  * [Список dailyPrintUsageSummariesByUser](/graph/api/reportroot-list-dailyprintusagesummariesbyuser?view=graph-rest-beta)
  * [Список monthlyPrintUsageSummariesByUser](/graph/api/reportroot-list-monthlyprintusagesummariesbyuser?view=graph-rest-beta)
  * [Список dailyPrintUsageSummariesByPrinter](/graph/api/reportroot-list-dailyprintusagesummariesbyprinter?view=graph-rest-beta)
  * [Список monthlyPrintUsageSummariesByPrinter](/graph/api/reportroot-list-monthlyprintusagesummariesbyprinter?view=graph-rest-beta)

* **Настройка разрешений для пользователей** через изменения в членстве пользователей и групп касательно принтеров:
  * [Список allowedUsers](/graph/api/printer-list-allowedusers?view=graph-rest-beta)
  * [Добавление allowedUser](/graph/api/printer-post-allowedusers?view=graph-rest-beta)
  * [Удаление allowedUser](/graph/api/printer-delete-alloweduser?view=graph-rest-beta)
  * [Список allowedGroups](/graph/api/printer-list-allowedgroups?view=graph-rest-beta)
  * [Добавление allowedGroup](/graph/api/printer-post-allowedgroups?view=graph-rest-beta)
  * [Удаление allowedGroup](/graph/api/printer-delete-allowedgroup?view=graph-rest-beta)

### <a name="seamlessly-replace-or-update-printer-hardware"></a>Комфорт при замене и обновлении оборудования для печати

Принтеры не видны пользователям до момента, когда они получают к ним [доступ](/graph/api/print-post-shares?view=graph-rest-beta). Это позволяет администраторам детально контролировать доступность определенного оборудования для печати в определенный момент времени.

При общем доступе к принтеру создается ресурс [printerShare](/graph/api/resources/printershare?view=graph-rest-beta), который в любой момент можно обновить для перевода на другой принтер, что упрощает замену неисправного оборудования для печати и отправку принтеров в текущий ремонт.

Чтобы применить эту возможность в своем приложении, перейдите в [Обновление printerShare](/graph/api/printershare-update?view=graph-rest-beta) и обновите ссылку `printer` на printerShare.

### <a name="extending-universal-print-to-support-pull-printing"></a>Расширение универсальной печати для поддержки печати по запросу

API универсальной печати Microsoft Graph позволяет приложению поддерживать печать по запросу. Чтобы настроить печать по запросу, необходимо зарегистрировать триггеры, уведомляющие приложение (через коммуникацию в рамках уведомления между службами), когда имеют место определенные события печати, такие как запуск задания печати.

Эти триггеры позволяют приложению прерывать рабочий процесс печати для выполнения таких задач, как перенаправление заданий на различные принтеры и изменение полезных данных документа.

Выполните следующие действия, чтобы включить печать по запросу:

1. [Создайте printTaskDefinition](/graph/api/print-post-taskdefinitions?view=graph-rest-beta) с помощью разрешений приложения. Это абстрактное определение задачи будет использоваться для создания задачи, которая будет содержать задание для вашего приложения. Необходимо определить по крайней мере одно определение задачи для каждого клиента, которое можно связать с любым количеством принтеров в клиенте с помощью триггеров задач (см. Шаг 4).

2. [Зарегистрируйте один виртуальный принтер или более](/graph/api/printer-create?view=graph-rest-beta) с помощью администраторского маркера проверки подлинности и `null` **physicalDeviceId**. "Виртуальный принтер" представляет собой объект принтера в Universal Print без прикрепленного физического устройства. Как правило, пользователи выполняют печать на виртуальных принтерах, а затем выбирают свои задания печати на физическом устройстве печати. См. шаг 6.

3. [Обновляйте атрибуты вашего виртуального принтера](/graph/api/printer-update?view=graph-rest-beta) с помощью разрешений приложения и типа носителя `application/ipp` (см. примеры).

4. [Создайте триггер задачи для вашего виртуального принтера](/graph/api/printer-post-tasktriggers?view=graph-rest-beta) с помощью администраторского маркера проверки подлинности, который будет использоваться для сопоставления определения задачи с виртуальным принтером.

5. При отправке задания печати на виртуальный принтер оно будет приостановлено по причине [printTaskTrigger](/graph/api/resources/printtasktrigger?view=graph-rest-beta). Будут созданы [printTask](/graph/api/resources/printtask?view=graph-rest-beta) с состоянием `processing` на основе связанного [printTaskDefinition](/graph/api/resources/printtaskdefinition?view=graph-rest-beta).

6. При прокрутке пользователем эмблемы на физическом принтере, принтер уведомит ваше приложение. В это время приложение может [получить задания связанного виртуального принтера](/graph/api/printer-list-jobs?view=graph-rest-beta) и отфильтровать список на задания, созданные текущим пользователем.

7. При выборе пользователем одного или нескольких заданий для печати, приложение может [перенаправить задание (-я) печати](/graph/api/printjob-redirect?view=graph-rest-beta) на физический принтер, и задание запустит печать. Вызов на перенаправление будет успешным только в том случае, если присутствует [printTask](/graph/api/resources/printtask?view=graph-rest-beta) в состоянии `processing` в связанном принтере, запущенном триггером, который был создан этим приложением в Шаге 4. После перенаправления задания, задача автоматически будет настроена на состояние `completed`.

   >**Примечание.** Приостановленные задания печати, не перенаправленные в течение двух дней, будут удалены.

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API универсальной печати в бета-версии Microsoft Graph](/graph/api/resources/print?view=graph-rest-beta)

## <a name="provide-feedback"></a>Предоставление отзывов

Мы будем рады узнать ваше мнение об API универсальной печати. Предоставьте свои предложения на сайте [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).

## <a name="see-also"></a>См. также

- [Что такое универсальная печать](https://docs.microsoft.com/universal-print/fundamentals/universal-print-whatis)
