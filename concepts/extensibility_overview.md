<span data-ttu-id="27fc6-p116">Для чтения или записи данных расширений в ресурсе необходимы те же [разрешения](./permissions_reference.md), что и для чтения или записи ресурса. Например, чтобы приложение могло добавить данные в профиль пользователя, который вошел в учетную запись, у него должно быть разрешение *User.ReadWrite.All*.</span><span class="sxs-lookup"><span data-stu-id="27fc6-p116">The same [permissions](./permissions_reference.md) that are required to read from or write to a specific resource are also required to read from or write to any extensions data on that resource.  For example, for an app to be able to update the signed-in user's profile with custom app data, the app must have been granted the *User.ReadWrite.All* permission.</span></span>

Для чтения или записи данных расширений в ресурсе необходимы те же [разрешения](./permissions_reference.md), что и для чтения или записи ресурса. Например, чтобы приложение могло добавить данные в профиль пользователя, который вошел в учетную запись, у него должно быть разрешение *User.ReadWrite.All*.

<span data-ttu-id="27fc6-229">Кроме того, для создания определений расширения схемы и управления ими приложению необходимо разрешение *Directory.AccessAsUser.All*.</span><span class="sxs-lookup"><span data-stu-id="27fc6-229">Additionally, to create and manage schema extension definitions, an application must be granted the *Directory.AccessAsUser.All* permission.</span></span>

## <a name="data-limits"></a><span data-ttu-id="27fc6-230">Ограничения данных</span><span class="sxs-lookup"><span data-stu-id="27fc6-230">Data limits</span></span>

### <a name="open-extension-limits"></a><span data-ttu-id="27fc6-231">Ограничения открытых расширений</span><span class="sxs-lookup"><span data-stu-id="27fc6-231">Open extension limits</span></span>
<span data-ttu-id="27fc6-232">К ресурсам каталогов, таким как **user**, **group**, **device**, применимы следующие ограничения:</span><span class="sxs-lookup"><span data-stu-id="27fc6-232">The following limits apply to directory resources (such as **user**, **group**, **device**):</span></span>

- <span data-ttu-id="27fc6-233">Каждое открытое расширение может содержать до 2 КБ данных (включая само определение расширения).</span><span class="sxs-lookup"><span data-stu-id="27fc6-233">Each open extension can have up to 2KB of data (including the extension definition itself).</span></span>
- <span data-ttu-id="27fc6-234">Приложение может создавать до двух открытых расширений для каждого экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="27fc6-234">An application can add up to two open extensions per resource instance.</span></span>

### <a name="schema-extension-limits"></a><span data-ttu-id="27fc6-235">Ограничения расширений схемы</span><span class="sxs-lookup"><span data-stu-id="27fc6-235">Schema extension limits</span></span>
<span data-ttu-id="27fc6-236">Приложение может создать не более пяти определений **расширений схемы**.</span><span class="sxs-lookup"><span data-stu-id="27fc6-236">An application may create no more than five **schema extension** definitions.</span></span>

## <a name="known-limitations"></a><span data-ttu-id="27fc6-237">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="27fc6-237">Known limitations</span></span>

<span data-ttu-id="27fc6-238">Об известных ограничениях на использование расширений можно узнать в [соответствующем разделе](known_issues.md#extensions) статьи об известных проблемах.</span><span class="sxs-lookup"><span data-stu-id="27fc6-238">For known limitations using extensions, see the [extensions section](known_issues.md#extensions) in the known issues article.</span></span>

## <a name="extension-examples"></a><span data-ttu-id="27fc6-239">Примеры расширений</span><span class="sxs-lookup"><span data-stu-id="27fc6-239">Extension examples</span></span>

[<span data-ttu-id="27fc6-240">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="27fc6-240">Add custom data to users using open extensions</span></span>](extensibility_open_users.md)

[<span data-ttu-id="27fc6-241">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="27fc6-241">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)

## <a name="see-also"></a><span data-ttu-id="27fc6-242">См. также</span><span class="sxs-lookup"><span data-stu-id="27fc6-242">See also</span></span>

[<span data-ttu-id="27fc6-243">Домены Office 365</span><span class="sxs-lookup"><span data-stu-id="27fc6-243">Office 365 domains</span></span>](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)

[<span data-ttu-id="27fc6-244">Добавление и подтверждение домена для клиента Office 365</span><span class="sxs-lookup"><span data-stu-id="27fc6-244">Adding and verifying a domain for an Office 365 tenant</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
